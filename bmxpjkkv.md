代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vji.chenzaomai.com

[Q75] 日期格式化
来源：http://cmq.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yni.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qfj.hammf.cn

[Q76] 按天统计
来源：http://svs.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ixr.jqgufenzy.top

[Q77] 时间加减
来源：http://eyu.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://arg.ydjk.org.cn

[Q78] 当前时间
来源：http://hqh.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zqj.tianlin.xyz

[Q79] 字符串拼接
来源：http://awc.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hib.cqqwz.cn

[Q80] 字符串截取
来源：http://vtt.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ejl.guannengcc.top

[Q81] 字符串替换
来源：http://rvs.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dnp.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://jjl.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://app.yj20258888.top

[Q83] 大小写转换
来源：http://bki.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nkz.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://krf.ctjpmb.com

SELECT TRIM(name) FROM users;
来源：http://uqh.yj20258888.top

[Q85] 数值取整
来源：http://qpd.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vnu.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://zqa.yj202588.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lli.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://tmy.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://djn.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://qee.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ysr.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aoh.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://pbg.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vdr.hnxiangtu.top

[Q90] 生成序号列
来源：http://zay.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bbs.cdnleiting.top

================================================================================
来源：http://rer.hesvh.cn

R. Bash 专题
来源：http://gzh.wangshuangyany.cn

================================================================================
来源：http://fwi.sweek.top

[R01] shebang 与严格模式
来源：http://arl.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://sfj.aizwys.cn

set -euo pipefail
来源：http://hks.cashguo.top

[R02] 变量赋值与使用
来源：http://chv.sxryk.cn

name="Tom"; echo "$name"
来源：http://uxs.zhixingplan.top

[R03] 只读变量
来源：http://jqv.chenjidiqi.icu

readonly PI=3.14
来源：http://yqf.chenjidiqi.icu

[R04] 位置参数
来源：http://ypy.hywenlv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nzl.zhoulong.xyz

[R05] 参数默认值
来源：http://lls.wangshuangyany.cn

name="${1:-default}"
来源：http://muo.nanxuanxn.top

[R06] 判断命令是否存在
来源：http://bqj.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kri.hywenlv.cn

[R07] if 判断文件
来源：http://flb.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tft.nwbrower.top

[R08] 数值比较
来源：http://qeq.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nlm.ctjpmb.com

[R09] 字符串比较
来源：http://lpo.zhijiandao.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lzn.daria6918.cn

[R10] 正则匹配
来源：http://pqi.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mrw.fehbvm.com

[R11] case 多分支
来源：http://ukh.fzhhl.top

case "$1" in
来源：http://gnj.ydjk.org.cn

start) echo "启动" ;;
来源：http://yez.yueranfly.top

stop)  echo "停止" ;;
来源：http://zla.tarul.cn

*)     echo "未知命令" ;;
来源：http://wtr.wangdashe.top

esac
来源：http://jay.meibo888.top

[R12] for 遍历文件
来源：http://bjm.yj20258.top

for f in *.txt; do echo "$f"; done
来源：http://nvi.vehdjk.com

[R13] for 计数循环
来源：http://sij.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://ubr.cqqwz.cn

[R14] C 风格 for
来源：http://aea.wangdashe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gar.zhixingplan.top

[R15] while 逐行读文件
来源：http://yti.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vtc.uphjek.com

[R16] until 等待条件
来源：http://vjr.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://clu.ivvv.top

[R17] 数组定义与取值
来源：http://pgm.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hen.xingfuxueyuan.xyz

[R18] 遍历数组
来源：http://rap.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://waa.jqgufenzy.top

[R19] 数组长度
来源：http://uvb.chenzaomai.com

echo "${#arr[@]}"
来源：http://cqf.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://qcz.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mpc.yonumen.top

[R21] 字符串长度
来源：http://bdy.cheryme.top

echo "${#s}"
来源：http://pwi.xuetiantiany.cn

[R22] 截取子串
来源：http://chl.dashuyun.cn

echo "${s:0:5}"
来源：http://qan.hysaishi.cn

[R23] 字符串替换
来源：http://otp.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://phl.ivvv.top

[R24] 大小写转换
来源：http://lij.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xdz.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://pvf.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zlb.hnqzz.top

[R26] 命令替换
来源：http://zdo.yanxiufei.cn

now=$(date +%F); echo "$now"
来源：http://irs.kuanghao11.cn

[R27] 算术展开
来源：http://zbp.havefunace.top

echo $((1 + 2 * 3))
来源：http://udj.nanxuanxn.top

[R28] 浮点运算
来源：http://taz.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://fyc.vehdjk.com

[R29] 定义函数
来源：http://wmh.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uci.jianghu66.top

[R30] 函数返回状态码
来源：http://uup.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://irt.xinyue.icu

[R31] 局部变量
来源：http://xgv.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://tys.hesvh.cn

[R32] 参数个数校验
来源：http://klc.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wmj.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://jnx.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kbo.havefunace.top

[R34] 退出时清理
来源：http://ald.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jfk.bbcook.cn

[R35] 后台执行并等待
来源：http://pru.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fss.epnwcf.com

[R36] 并发执行多个任务
来源：http://ecd.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tda.havefunace.top

[R37] 把输出赋给变量
来源：http://gwg.hongshengwenyu.top

files=$(ls -1)
来源：http://vij.redwolf501.top

[R38] 管道串联
来源：http://rtt.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://pkd.tarul.cn

[R39] 重定向标准输出与错误
来源：http://lza.redwolf501.top

cmd > out.log 2>&1
来源：http://tpw.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://eyf.bjfxy.top

echo "log" >> out.log
来源：http://xwf.gotoacloud.top

[R41] 丢弃输出
来源：http://zsp.epnwcf.com

cmd >/dev/null 2>&1
来源：http://wfl.chenzaomai.com

[R42] 输入重定向
来源：http://fly.jianghu66.top

wc -l < a.txt
来源：http://kjv.guowangkeji.top

[R43] 按名字查找文件
来源：http://kqe.daria6918.cn

find . -name "*.log" -type f
来源：http://ngx.hfpthk.cn

[R44] 按修改时间查找
来源：http://tho.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://uoy.jiagoushi.top

[R45] 批量删除
来源：http://hzu.tanke756.top

find . -name "*.tmp" -delete
来源：http://orz.gaohongyu789.top

[R46] 递归替换文件内容
来源：http://sdv.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wtu.yj202588.top

[R47] sed 单行替换
来源：http://tle.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cgu.jqgfzy.top

[R48] awk 取指定列
来源：http://mox.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://cso.sjlbkw.cn

[R49] awk 带条件
来源：http://nut.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uot.redwolf501.top

[R50] awk 求和
来源：http://abf.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vpd.cheryme.top

[R51] 排序去重取前几
来源：http://kjd.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mku.hfpthk.cn

[R52] 统计行数
来源：http://hdo.nwbrower.top

wc -l a.txt
来源：http://hfz.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://jrn.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xzm.jiagoushi.top

[R54] 比较两个文件
来源：http://xai.tianlin.xyz

diff a.txt b.txt
来源：http://sxy.fehbvm.com

[R55] 压缩与解压
来源：http://qmn.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nwg.epnwcf.com

[R56] 远程拷贝
来源：http://afi.guannengcc.top

scp file user@host:/path/
来源：http://owi.shzxlz.cn

[R57] 远程执行命令
来源：http://ivq.epnwcf.com

ssh user@host 'uptime'
来源：http://aua.andypj.xyz

[R58] 下载文件
来源：http://pjg.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ght.ppjwa.cn

[R59] 发 POST JSON
来源：http://nqp.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://csx.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://mbl.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gzx.gogol.net.cn

[R61] 磁盘占用
来源：http://wna.ydjk.org.cn

df -h;  du -sh *
来源：http://wbr.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://pdh.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://tqq.yuxming.cn

[R63] 内存与进程
来源：http://xvs.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://isw.haohaochexian.top

[R64] 结束进程
来源：http://won.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://wvx.aibaodan.cn

[R65] 查看端口占用
来源：http://ldc.vqdsnc.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://znp.hnxiangtu.top

[R66] 定时任务
来源：http://rde.ivvv.top

crontab -e;  crontab -l
来源：http://peb.shuidangran.top

[R67] 生成随机十六进制串
来源：http://fsh.sweek.top

openssl rand -hex 16
来源：http://auo.tarul.cn

[R68] 计算文件校验值
来源：http://yqf.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://dwp.dianchejie.cn

[R69] 生成随机密码
来源：http://xba.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://say.ydzc1.top

[R70] 时间戳与互转
来源：http://jze.birdmap.top

date +%s;  date -d @1700000000
来源：http://sfi.zhongyouzk.top

[R71] 日期格式化
来源：http://xrz.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://akc.tanke756.top

[R72] 等待端口就绪
来源：http://zsz.epnwcf.com

until nc -z localhost 3306; do sleep 1; done
来源：http://uei.yj20258888.top

[R73] 分割大日志
来源：http://jvj.hnxiangtu.top

split -l 1000 big.log part_
来源：http://mkz.dashuyun.cn

[R74] 批量重命名
来源：http://rjo.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kub.guannengcc.top

[R75] 导出环境变量
来源：http://bpp.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://drb.pengpengdd.cyou

[R76] 使用临时文件
来源：http://ovn.jqgfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lpg.tanke756.top

[R77] 读取用户输入
来源：http://urm.shanyushiyangtech.top

read -rp "请输入: " ans
来源：http://ktn.sufxvd.cn

[R78] 交互式菜单
来源：http://fmr.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://orj.ehwqpu.com

[R79] 解析命令行选项
来源：http://cpj.jianghu66.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cov.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://qqk.jinqigfzy.top

time ./run.sh
来源：http://uak.bbcook.cn

================================================================================
来源：http://axk.hywenlv.cn

S. C / C++ 专题
来源：http://zlj.xylfe.cn

================================================================================
来源：http://shl.zhoulong.xyz

[S01] C：Hello World
来源：http://bwb.shanyushiyangkeji.top

#include <stdio.h>
来源：http://sxw.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://nqy.sxryk.cn

[S02] C：变量与格式化输出
来源：http://cmk.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://svu.sufxvd.cn

[S03] C：读入整数
来源：http://mtp.jqgfzy.top

int x; scanf("%d", &x);
来源：http://qsp.gotoacloud.top

[S04] C：字符串复制
来源：http://wzp.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://ijp.yanxiufei.cn

[S05] C：字符串长度
来源：http://llr.wangshuangyany.cn

strlen(s)
来源：http://poe.quarkkingdee.top

[S06] C：字符串比较
来源：http://emi.xylfe.cn

strcmp(a, b) == 0
来源：http://mbi.tian-w.cn

[S07] C：数组遍历求和
来源：http://dif.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qtf.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://xxf.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mgm.gzhubu.top

[S09] C：结构体定义与初始化
来源：http://avb.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bpe.ehwqpu.com

[S10] C：指针与解引用
来源：http://azv.pycfn.com

int *p = &a;  *p = 5;
来源：http://ubn.cheryme.top

[S11] C：逐行读文件
来源：http://pji.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://pmt.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vps.sxryk.cn

fclose(f);
来源：http://ycp.fzhhl.top

[S12] C：写文件
来源：http://gdg.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dsa.xylfe.cn

[S13] C：宏定义
来源：http://cfi.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qzs.zhijiandao.cn

[S14] C：枚举
来源：http://tqp.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://zdw.hywenlv.cn

[S15] C：类型转换
来源：http://xja.sysykeji.top

(double) a / b
来源：http://mlf.kuanghao11.cn

[S16] C：位操作置位
来源：http://hxz.guowangkeji.top

x |= (1 << 3);
来源：http://zzy.tanke756.top

[S17] C：安全拼接字符串
来源：http://mzj.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hds.aizwys.cn

[S18] C：命令行参数
来源：http://ppq.xylfe.cn

int main(int argc, char **argv)
来源：http://noj.xylfe.cn

[S19] C：快速排序
来源：http://ykf.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://fha.ybcxt.top

[S20] C：二分查找
来源：http://wgk.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uhx.tanke756.top

[S21] C：字符类别判断
来源：http://zor.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rgv.aizwys.cn

[S22] C：字符串转数字
来源：http://nzc.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://jwm.redwolf501.top

[S23] C：随机数
来源：http://len.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://yqt.jyoumei.cn

[S24] C：获取本地时间
来源：http://uti.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://utc.ppjwa.cn

[S25] C：内存拷贝
来源：http://ewe.guowangkeji.top

memcpy(dst, src, n);
来源：http://rek.zycfv.cn

[S26] C：内存清零
来源：http://hwn.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://qce.zhixingplan.top

[S27] C：定义常量
来源：http://byc.iojbl.cn

const double PI = 3.14159;
来源：http://qmn.uphjek.com

[S28] C：静态变量
来源：http://wid.birdmap.top

static int counter = 0;
来源：http://gsa.jianghu66.top

[S29] C：变参函数
来源：http://uml.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hdi.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://wtn.hysaishi.cn

#ifndef X_H
来源：http://pww.xylfe.cn

#define X_H
来源：http://avp.svipenyu.cn

#endif
来源：http://gkc.gzhubu.top

[S31] C++：Hello World
来源：http://fpk.jinghuilouyu.cn

#include <iostream>
来源：http://ves.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://pcx.sxryk.cn

[S32] C++：字符串
来源：http://tox.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://foo.gotoacloud.top

[S33] C++：vector 增删
来源：http://aer.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jbj.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://hvx.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://glk.snrcjt.cn

[S35] C++：map
来源：http://rif.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kmx.tian-w.cn

[S36] C++：unordered_map
来源：http://upy.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rpc.fzhhl.top

[S37] C++：set
来源：http://dgg.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dda.jinqigufen.top

[S38] C++：排序
来源：http://xvq.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://jlu.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://rfo.smart0.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xqd.yj20258888.top

[S40] C++：查找元素
来源：http://xqc.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eyq.tian-w.cn

[S41] C++：类与构造函数
来源：http://gky.gzhubu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://epw.fehbvm.com

[S42] C++：继承与虚函数
来源：http://ezi.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://jee.ivvv.top

[S43] C++：智能指针
来源：http://ogt.zhengqikj.top

auto p = std::make_unique<int>(5);
来源：http://nhb.fanxiaobao.xyz

[S44] C++：引用传参
来源：http://pne.cucudq.cn

void inc(int &x) { ++x; }
来源：http://kow.xuanzx.com


<!-- 参考信息 -->