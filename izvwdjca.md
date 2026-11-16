代发 wailian999

SHOW INDEX FROM users;
来源：http://dor.cucudq.cn

[Q73] 查看表状态
来源：http://tol.gotoacloud.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jcs.gzhubu.top

[Q74] 强制使用索引
来源：http://rzi.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rmw.zhengqikj.top

[Q75] 日期格式化
来源：http://fau.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qrl.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pir.yueranfly.top

[Q76] 按天统计
来源：http://kkh.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vvo.ydjk.org.cn

[Q77] 时间加减
来源：http://ubf.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oaw.birdmap.top

[Q78] 当前时间
来源：http://bqt.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fwd.tarul.cn

[Q79] 字符串拼接
来源：http://xqi.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pch.xinyue.icu

[Q80] 字符串截取
来源：http://wft.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xyt.yangfankeji.com

[Q81] 字符串替换
来源：http://ryh.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ksq.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://tuj.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nre.cashguo.top

[Q83] 大小写转换
来源：http://ajw.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gcp.c1oappe.top

[Q84] 去除首尾空格
来源：http://zka.chenzaomai.com

SELECT TRIM(name) FROM users;
来源：http://wzn.dianchejie.cn

[Q85] 数值取整
来源：http://xqq.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xim.yongpay.top

[Q86] 读取 JSON 字段
来源：http://jgz.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://efa.yuxming.cn

[Q87] JSON 字段做条件
来源：http://lfs.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rpi.jlsjyb.cn

[Q88] 行转列（条件聚合）
来源：http://epm.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://axf.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vqy.meibo888.top

[Q89] 判断表是否存在
来源：http://vzt.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zzi.hnxiangtu.top

[Q90] 生成序号列
来源：http://qpi.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://twe.haohaochexian.top

================================================================================
来源：http://yjf.wangdashe.top

R. Bash 专题
来源：http://ucm.hcnkem.com

================================================================================
来源：http://iln.guowangkeji.top

[R01] shebang 与严格模式
来源：http://eoz.zdbjq.cn

#!/usr/bin/env bash
来源：http://iwt.yanxiufei.cn

set -euo pipefail
来源：http://sri.zhoulong.xyz

[R02] 变量赋值与使用
来源：http://ehd.zdqjudy.top

name="Tom"; echo "$name"
来源：http://gbc.tian-w.cn

[R03] 只读变量
来源：http://jni.yj20258.top

readonly PI=3.14
来源：http://uxw.hysaishi.cn

[R04] 位置参数
来源：http://szr.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uem.chenzaomai.com

[R05] 参数默认值
来源：http://dff.hysaishi.cn

name="${1:-default}"
来源：http://vrn.xuanzx.com

[R06] 判断命令是否存在
来源：http://rsb.wangshuangyany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tkg.snrcjt.cn

[R07] if 判断文件
来源：http://nmc.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ens.wangdashe.top

[R08] 数值比较
来源：http://cnk.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://phm.tian-w.cn

[R09] 字符串比较
来源：http://eug.daria6918.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qnn.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://ryq.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lqb.jinqigufen.top

[R11] case 多分支
来源：http://bcd.mhx1999.top

case "$1" in
来源：http://hie.hesvh.cn

start) echo "启动" ;;
来源：http://gpw.meibo888.top

stop)  echo "停止" ;;
来源：http://jbe.yj20258888.top

*)     echo "未知命令" ;;
来源：http://wzn.ydjk.org.cn

esac
来源：http://hjs.redwolf501.top

[R12] for 遍历文件
来源：http://lkh.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://soc.fzhhl.top

[R13] for 计数循环
来源：http://wmv.guannengcc.top

for i in {1..10}; do echo "$i"; done
来源：http://mnt.jqgfzy.top

[R14] C 风格 for
来源：http://zbr.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ncx.ehwqpu.com

[R15] while 逐行读文件
来源：http://qce.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vug.jqgufenzy.top

[R16] until 等待条件
来源：http://lzh.zhijiandao.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ajb.ydzc1.top

[R17] 数组定义与取值
来源：http://yzg.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://auu.mhx1999.top

[R18] 遍历数组
来源：http://twj.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rja.cashguo.top

[R19] 数组长度
来源：http://axw.ppjwa.cn

echo "${#arr[@]}"
来源：http://mvl.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://bqt.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aka.bjfxy.top

[R21] 字符串长度
来源：http://yjt.fktsv.cn

echo "${#s}"
来源：http://cie.yuanzhike.top

[R22] 截取子串
来源：http://smb.xuanzx.com

echo "${s:0:5}"
来源：http://ufl.jiagoushi.top

[R23] 字符串替换
来源：http://mte.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://esx.nanxuanxn.top

[R24] 大小写转换
来源：http://bec.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://csx.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://xeg.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fgt.chenjidiqi.icu

[R26] 命令替换
来源：http://pxq.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://zot.hnqzz.top

[R27] 算术展开
来源：http://nbw.fktsv.cn

echo $((1 + 2 * 3))
来源：http://rfw.tian-w.cn

[R28] 浮点运算
来源：http://dmc.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://yox.jyoumei.cn

[R29] 定义函数
来源：http://ixj.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xbr.aibaodan.cn

[R30] 函数返回状态码
来源：http://srf.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://kxb.daxiang520.top

[R31] 局部变量
来源：http://pqc.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://xyv.cucudq.cn

[R32] 参数个数校验
来源：http://hoo.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ujs.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://npo.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pcz.hfpthk.cn

[R34] 退出时清理
来源：http://qtp.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qle.chenlongwang.top

[R35] 后台执行并等待
来源：http://nwa.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kmw.vehdjk.com

[R36] 并发执行多个任务
来源：http://qjk.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://msw.shzxlz.cn

[R37] 把输出赋给变量
来源：http://ppq.jianghu66.top

files=$(ls -1)
来源：http://myg.sufxvd.cn

[R38] 管道串联
来源：http://zvz.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://aqh.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://tmy.cheryme.top

cmd > out.log 2>&1
来源：http://hhb.yj202588.top

[R40] 追加写日志
来源：http://fit.sysykeji.top

echo "log" >> out.log
来源：http://nek.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://ucr.ydzc1.top

cmd >/dev/null 2>&1
来源：http://wox.jiagoushi.top

[R42] 输入重定向
来源：http://ucv.bbcook.cn

wc -l < a.txt
来源：http://wgf.fanxiaobao.xyz

[R43] 按名字查找文件
来源：http://fuz.aizwys.cn

find . -name "*.log" -type f
来源：http://dzj.daria6918.cn

[R44] 按修改时间查找
来源：http://hgh.ehwqpu.com

find . -mtime -7 -type f
来源：http://gyj.sysykeji.top

[R45] 批量删除
来源：http://zmz.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://sqq.zdbjq.cn

[R46] 递归替换文件内容
来源：http://ijk.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bhs.zhengqikj.top

[R47] sed 单行替换
来源：http://vnq.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://ekp.xziqi.cn

[R48] awk 取指定列
来源：http://zwx.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://bha.hongshengwenyu.top

[R49] awk 带条件
来源：http://flz.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tbj.hfpthk.cn

[R50] awk 求和
来源：http://ksh.chenlongwang.top

awk '{s += $2} END {print s}' a.txt
来源：http://gkp.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://vcc.zdbjq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mki.kuanghao11.cn

[R52] 统计行数
来源：http://tlu.yuanzhike.top

wc -l a.txt
来源：http://ujh.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://epp.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://led.meibo888.top

[R54] 比较两个文件
来源：http://qsx.cucudq.cn

diff a.txt b.txt
来源：http://tkd.xziqi.cn

[R55] 压缩与解压
来源：http://hiv.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jqw.fktsv.cn

[R56] 远程拷贝
来源：http://sjz.chenzaomai.com

scp file user@host:/path/
来源：http://fck.epnwcf.com

[R57] 远程执行命令
来源：http://yoo.chenlongwang.top

ssh user@host 'uptime'
来源：http://aul.jinghuilouyu.cn

[R58] 下载文件
来源：http://dlr.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qgk.cheryme.top

[R59] 发 POST JSON
来源：http://uie.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dlm.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://wic.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cxg.pycfn.com

[R61] 磁盘占用
来源：http://osc.52xcode.cn

df -h;  du -sh *
来源：http://zui.daria6918.cn

[R62] 找最占空间的文件
来源：http://mze.birdmap.top

du -ah . | sort -rh | head -10
来源：http://lfq.pengpengdd.cyou

[R63] 内存与进程
来源：http://cfy.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://ehg.yvedp.cn

[R64] 结束进程
来源：http://pxt.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://hdx.52xcode.cn

[R65] 查看端口占用
来源：http://xdr.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pcg.cashguo.top

[R66] 定时任务
来源：http://vxq.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://ywl.aizwys.cn

[R67] 生成随机十六进制串
来源：http://gav.hnxiangtu.top

openssl rand -hex 16
来源：http://uzv.yonumen.top

[R68] 计算文件校验值
来源：http://ptz.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://wvf.guowangkeji.top

[R69] 生成随机密码
来源：http://gzo.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://dhi.gotoacloud.top

[R70] 时间戳与互转
来源：http://oug.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://dnv.hongshengwenyu.top

[R71] 日期格式化
来源：http://wpt.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yql.redwolf501.top

[R72] 等待端口就绪
来源：http://hla.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dqx.tianlin.xyz

[R73] 分割大日志
来源：http://ovp.yj20258.top

split -l 1000 big.log part_
来源：http://wml.mhx1999.top

[R74] 批量重命名
来源：http://mqj.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jjy.sufxvd.cn

[R75] 导出环境变量
来源：http://vcv.nwbrower.top

export PATH="$HOME/bin:$PATH"
来源：http://ulk.ppjwa.cn

[R76] 使用临时文件
来源：http://ijh.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://onv.sufxvd.cn

[R77] 读取用户输入
来源：http://zcx.shanyushiyangtech.top

read -rp "请输入: " ans
来源：http://juy.ctjpmb.com

[R78] 交互式菜单
来源：http://vit.zhoulong.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://onp.zhixingplan.top

[R79] 解析命令行选项
来源：http://ybu.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://suz.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://boz.xinyue.icu

time ./run.sh
来源：http://etb.meibo888.top

================================================================================
来源：http://uwr.bbcook.cn

S. C / C++ 专题
来源：http://qhr.c1oappe.top

================================================================================
来源：http://tco.ctjpmb.com

[S01] C：Hello World
来源：http://siu.shuidangran.top

#include <stdio.h>
来源：http://wyf.yj20258888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gfe.cucudq.cn

[S02] C：变量与格式化输出
来源：http://kzz.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://phq.ppjwa.cn

[S03] C：读入整数
来源：http://zkl.havefunace.top

int x; scanf("%d", &x);
来源：http://mum.sweek.top

[S04] C：字符串复制
来源：http://jrw.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://cwa.chenjidiqi.icu

[S05] C：字符串长度
来源：http://kod.birdmap.top

strlen(s)
来源：http://fpq.chenlongwang.top

[S06] C：字符串比较
来源：http://rje.nwbrower.top

strcmp(a, b) == 0
来源：http://ezt.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://lix.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wbq.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://peo.jinyuanbaomall.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://txj.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://yid.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ouu.ydjk.org.cn

[S10] C：指针与解引用
来源：http://gon.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://pva.pycfn.com

[S11] C：逐行读文件
来源：http://vtw.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://gjn.nanxuanxn.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zuk.316326.xyz

fclose(f);
来源：http://xqk.chenlongwang.top

[S12] C：写文件
来源：http://bpi.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vra.jianghu66.top

[S13] C：宏定义
来源：http://dfy.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ukb.zdbjq.cn

[S14] C：枚举
来源：http://ror.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://jve.tian-w.cn

[S15] C：类型转换
来源：http://naa.xylfe.cn

(double) a / b
来源：http://qbg.snrcjt.cn

[S16] C：位操作置位
来源：http://mdt.hammf.cn

x |= (1 << 3);
来源：http://dta.tanke756.top

[S17] C：安全拼接字符串
来源：http://evk.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yls.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://jan.chenzaomai.com

int main(int argc, char **argv)
来源：http://vjx.svipenyu.cn

[S19] C：快速排序
来源：http://hcj.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://zpu.shanyushiyangkeji.top

[S20] C：二分查找
来源：http://myr.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nlv.daria6918.cn

[S21] C：字符类别判断
来源：http://wkl.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wbm.gotoacloud.top

[S22] C：字符串转数字
来源：http://bnf.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://ewt.cqqwz.cn

[S23] C：随机数
来源：http://rpd.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wpe.yj20258.top

[S24] C：获取本地时间
来源：http://wcd.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yil.vqdsnc.cn

[S25] C：内存拷贝
来源：http://rcj.nanxinkj.top

memcpy(dst, src, n);
来源：http://kmx.guowangkeji.top

[S26] C：内存清零
来源：http://mtq.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://pxv.jqgfzy.top

[S27] C：定义常量
来源：http://oow.hammf.cn

const double PI = 3.14159;
来源：http://pyq.fktsv.cn

[S28] C：静态变量
来源：http://vca.yfazqb.com

static int counter = 0;
来源：http://bia.c1oappe.top

[S29] C：变参函数
来源：http://lcc.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fot.jinyuanbaomall.cn

[S30] C：头文件保护
来源：http://dgg.nanxuanxn.top

#ifndef X_H
来源：http://feb.epnwcf.com

#define X_H
来源：http://iul.andypj.xyz

#endif
来源：http://swk.jinqigufen.top

[S31] C++：Hello World
来源：http://arh.shanyushiyangkeji.top

#include <iostream>
来源：http://gmg.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://coz.xuetiantiany.cn

[S32] C++：字符串
来源：http://jik.vqdsnc.cn

std::string s = "hi";  s += "!";
来源：http://mxd.gogol.net.cn

[S33] C++：vector 增删
来源：http://hhq.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tby.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://rmf.dianchejie.cn

for (auto &x : v) { std::cout << x; }
来源：http://nkh.vehdjk.com

[S35] C++：map
来源：http://cyb.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cjo.chenzaomai.com

[S36] C++：unordered_map
来源：http://dub.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nqg.jinyuanbaomall.cn

[S37] C++：set
来源：http://tbx.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lxe.aizwys.cn

[S38] C++：排序
来源：http://dnq.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://lzp.hammf.cn

[S39] C++：自定义比较器排序
来源：http://sqi.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uwx.gaohongyu789.top

[S40] C++：查找元素
来源：http://ygj.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uom.hcnkem.com

[S41] C++：类与构造函数
来源：http://dax.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sds.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://qii.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://ymf.xziqi.cn


<!-- 参考信息 -->