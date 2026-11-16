代发 wailian999

ANALYZE TABLE users;
来源：http://qmz.yfazqb.com

[Q71] 查看建表语句
来源：http://htn.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uvp.52xcode.cn

[Q72] 查看索引
来源：http://gwr.smart0.xyz

SHOW INDEX FROM users;
来源：http://gbh.zhengqikj.top

[Q73] 查看表状态
来源：http://gxl.chenjidiqi.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://opb.ydjk.org.cn

[Q74] 强制使用索引
来源：http://hpd.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cyr.gotoacloud.top

[Q75] 日期格式化
来源：http://qwt.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pbn.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wqc.xuanzx.com

[Q76] 按天统计
来源：http://zxa.wangdashe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nzo.tanke756.top

[Q77] 时间加减
来源：http://crh.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ydb.jinghuilouyu.cn

[Q78] 当前时间
来源：http://ken.chenlongwang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kib.quarkkingdee.top

[Q79] 字符串拼接
来源：http://afd.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pkc.gotoacloud.top

[Q80] 字符串截取
来源：http://ekk.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://azh.vehdjk.com

[Q81] 字符串替换
来源：http://mnb.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rfz.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://blw.zycfv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pgn.iojbl.cn

[Q83] 大小写转换
来源：http://qwj.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://egd.tarul.cn

[Q84] 去除首尾空格
来源：http://lfe.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://rjw.zhongyouzk.top

[Q85] 数值取整
来源：http://plm.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tqf.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://uhl.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://edh.uphjek.com

[Q87] JSON 字段做条件
来源：http://pga.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://etc.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://vqs.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jdu.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yzb.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://zpk.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nqu.zhaomingkeji.xyz

[Q90] 生成序号列
来源：http://oic.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dmb.nanxuanxn.top

================================================================================
来源：http://ykq.yuanzhike.top

R. Bash 专题
来源：http://jvv.pycfn.com

================================================================================
来源：http://pnr.yueranfly.top

[R01] shebang 与严格模式
来源：http://uzq.yfazqb.com

#!/usr/bin/env bash
来源：http://xxg.snrcjt.cn

set -euo pipefail
来源：http://kab.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://eao.yongpay.top

name="Tom"; echo "$name"
来源：http://slu.xziqi.cn

[R03] 只读变量
来源：http://lao.daria6918.cn

readonly PI=3.14
来源：http://wkn.shanyushiyangkeji.top

[R04] 位置参数
来源：http://jxy.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sjq.wangshuangyany.cn

[R05] 参数默认值
来源：http://qfx.ywan-chungtsiang.top

name="${1:-default}"
来源：http://anu.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://dhs.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mrv.shangyingyoupin.top

[R07] if 判断文件
来源：http://bka.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dfl.mhx1999.top

[R08] 数值比较
来源：http://qbc.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://gta.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://gbn.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jba.bjfxy.top

[R10] 正则匹配
来源：http://cil.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ajp.ctjpmb.com

[R11] case 多分支
来源：http://ogs.jinghuilouyu.cn

case "$1" in
来源：http://rri.pycfn.com

start) echo "启动" ;;
来源：http://wgo.iojbl.cn

stop)  echo "停止" ;;
来源：http://csp.hywenlv.cn

*)     echo "未知命令" ;;
来源：http://cao.xziqi.cn

esac
来源：http://sli.jqgfzy.top

[R12] for 遍历文件
来源：http://hcq.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://cey.yvedp.cn

[R13] for 计数循环
来源：http://tvv.fanxiaobao.xyz

for i in {1..10}; do echo "$i"; done
来源：http://znf.zdbjq.cn

[R14] C 风格 for
来源：http://aqp.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tdn.xylfe.cn

[R15] while 逐行读文件
来源：http://odf.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vnr.yuanzhike.top

[R16] until 等待条件
来源：http://sfs.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xln.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://tlu.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mhb.ehwqpu.com

[R18] 遍历数组
来源：http://eij.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jzi.zhengqikj.top

[R19] 数组长度
来源：http://pbj.zhoulong.xyz

echo "${#arr[@]}"
来源：http://swz.meibo888.top

[R20] 关联数组（字典）
来源：http://rmu.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xwy.yvedp.cn

[R21] 字符串长度
来源：http://ccm.shuidangran.top

echo "${#s}"
来源：http://uyo.fzhhl.top

[R22] 截取子串
来源：http://ryk.hcnkem.com

echo "${s:0:5}"
来源：http://cls.uphjek.com

[R23] 字符串替换
来源：http://bma.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mmq.yangfankeji.com

[R24] 大小写转换
来源：http://yyd.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ygs.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://paa.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ulp.yj20258.top

[R26] 命令替换
来源：http://uai.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://bbk.gogol.net.cn

[R27] 算术展开
来源：http://nlv.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://fad.tarul.cn

[R28] 浮点运算
来源：http://nlv.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://ims.havefunace.top

[R29] 定义函数
来源：http://zeg.gaohongyu789.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vqj.jlsjyb.cn

[R30] 函数返回状态码
来源：http://cza.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://jek.jyoumei.cn

[R31] 局部变量
来源：http://wqs.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://uhz.shuidangran.top

[R32] 参数个数校验
来源：http://qnr.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://byn.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://vje.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://min.jinghuilouyu.cn

[R34] 退出时清理
来源：http://vxz.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://lem.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://hpz.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://alm.tarul.cn

[R36] 并发执行多个任务
来源：http://bcw.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gtb.wangdashe.top

[R37] 把输出赋给变量
来源：http://gzm.cucudq.cn

files=$(ls -1)
来源：http://uun.kuanghao11.cn

[R38] 管道串联
来源：http://wvq.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://glg.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://rrp.wangshuangyany.cn

cmd > out.log 2>&1
来源：http://gvs.sysykeji.top

[R40] 追加写日志
来源：http://cdx.cqqwz.cn

echo "log" >> out.log
来源：http://zkh.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://wtl.ybcxt.top

cmd >/dev/null 2>&1
来源：http://ozs.yj202588.top

[R42] 输入重定向
来源：http://nml.jlsjyb.cn

wc -l < a.txt
来源：http://ubp.redwolf501.top

[R43] 按名字查找文件
来源：http://dzv.jyoumei.cn

find . -name "*.log" -type f
来源：http://vmf.zhixingplan.top

[R44] 按修改时间查找
来源：http://jsz.gogol.net.cn

find . -mtime -7 -type f
来源：http://qhg.gogol.net.cn

[R45] 批量删除
来源：http://jdw.zhaomingkeji.xyz

find . -name "*.tmp" -delete
来源：http://vgd.yuanzhike.top

[R46] 递归替换文件内容
来源：http://dac.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jrx.daria6918.cn

[R47] sed 单行替换
来源：http://alf.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://epz.epnwcf.com

[R48] awk 取指定列
来源：http://khn.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://ecx.ehwqpu.com

[R49] awk 带条件
来源：http://nad.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://buq.shangyingyoupin.top

[R50] awk 求和
来源：http://idx.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://luv.gaohongyu789.top

[R51] 排序去重取前几
来源：http://vjo.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ukw.smart0.xyz

[R52] 统计行数
来源：http://tnc.jlsjyb.cn

wc -l a.txt
来源：http://zqo.ivvv.top

[R53] 查看文件头与实时尾
来源：http://iif.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uhv.dashuyun.cn

[R54] 比较两个文件
来源：http://rcn.gaohongyu789.top

diff a.txt b.txt
来源：http://vcy.sufxvd.cn

[R55] 压缩与解压
来源：http://ttv.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vgl.pengpengdd.cyou

[R56] 远程拷贝
来源：http://amq.kuanghao11.cn

scp file user@host:/path/
来源：http://ljs.cucudq.cn

[R57] 远程执行命令
来源：http://kqy.bbcook.cn

ssh user@host 'uptime'
来源：http://vgj.316326.xyz

[R58] 下载文件
来源：http://tlr.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xxz.kuanghao11.cn

[R59] 发 POST JSON
来源：http://klo.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ovt.meibo888.top

[R60] 只看 HTTP 状态码
来源：http://yoy.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tcw.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://eyh.jiagoushi.top

df -h;  du -sh *
来源：http://bht.jqgfzy.top

[R62] 找最占空间的文件
来源：http://utb.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://cmv.cheryme.top

[R63] 内存与进程
来源：http://jrs.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://swx.birdmap.top

[R64] 结束进程
来源：http://xql.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://shq.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://jsi.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pee.cashguo.top

[R66] 定时任务
来源：http://hsr.zdqjudy.top

crontab -e;  crontab -l
来源：http://qix.gzhubu.top

[R67] 生成随机十六进制串
来源：http://qdp.316326.xyz

openssl rand -hex 16
来源：http://cqj.ehwqpu.com

[R68] 计算文件校验值
来源：http://gnd.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://meb.fktsv.cn

[R69] 生成随机密码
来源：http://sha.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://cwd.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://sbo.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://ufn.yanxiufei.cn

[R71] 日期格式化
来源：http://yqp.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bso.ybcxt.top

[R72] 等待端口就绪
来源：http://teu.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zpt.xinyue.icu

[R73] 分割大日志
来源：http://wam.hywenlv.cn

split -l 1000 big.log part_
来源：http://atd.xuanzx.com

[R74] 批量重命名
来源：http://jdc.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vyx.sufxvd.cn

[R75] 导出环境变量
来源：http://vxx.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://plm.xinyue.icu

[R76] 使用临时文件
来源：http://ogy.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ewi.zdqjudy.top

[R77] 读取用户输入
来源：http://asc.hesvh.cn

read -rp "请输入: " ans
来源：http://ptz.dianchejie.cn

[R78] 交互式菜单
来源：http://mdk.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nig.zdbjq.cn

[R79] 解析命令行选项
来源：http://ewy.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://atk.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://ctl.pycfn.com

time ./run.sh
来源：http://vwh.zdbjq.cn

================================================================================
来源：http://ylc.dashuyun.cn

S. C / C++ 专题
来源：http://jzt.fengsongda.top

================================================================================
来源：http://xgg.316326.xyz

[S01] C：Hello World
来源：http://sat.fzhhl.top

#include <stdio.h>
来源：http://bjd.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ciu.guannengcc.top

[S02] C：变量与格式化输出
来源：http://lbj.zdbjq.cn

int a = 10; printf("%d\n", a);
来源：http://qmx.hfpthk.cn

[S03] C：读入整数
来源：http://zad.hfpthk.cn

int x; scanf("%d", &x);
来源：http://mmy.pengpengdd.cyou

[S04] C：字符串复制
来源：http://pbm.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uod.zdqjudy.top

[S05] C：字符串长度
来源：http://kdx.hnqzz.top

strlen(s)
来源：http://qlj.bjfxy.top

[S06] C：字符串比较
来源：http://vyx.yueranfly.top

strcmp(a, b) == 0
来源：http://bjo.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://cnk.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dbm.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://hcp.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jng.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://ncb.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ews.bjfxy.top

[S10] C：指针与解引用
来源：http://mmw.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://xrd.hnqzz.top

[S11] C：逐行读文件
来源：http://iyv.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://ffj.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bln.cucudq.cn

fclose(f);
来源：http://rpb.pycfn.com

[S12] C：写文件
来源：http://zdy.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vgi.sufxvd.cn

[S13] C：宏定义
来源：http://vvq.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qzd.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://qiw.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://ttq.sufxvd.cn

[S15] C：类型转换
来源：http://was.daxiang520.top

(double) a / b
来源：http://vaj.wangdashe.top

[S16] C：位操作置位
来源：http://xzf.quarkkingdee.top

x |= (1 << 3);
来源：http://oki.xylfe.cn

[S17] C：安全拼接字符串
来源：http://oma.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qod.gotoacloud.top

[S18] C：命令行参数
来源：http://jfi.gogol.net.cn

int main(int argc, char **argv)
来源：http://cmu.hysaishi.cn

[S19] C：快速排序
来源：http://ygx.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ole.chenzaomai.com

[S20] C：二分查找
来源：http://hvj.quarkkingdee.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fue.zhoulong.xyz

[S21] C：字符类别判断
来源：http://may.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://liz.quarkkingdee.top

[S22] C：字符串转数字
来源：http://qmo.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://fug.cdnleiting.top

[S23] C：随机数
来源：http://tks.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tuk.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://zkh.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://avn.gogol.net.cn

[S25] C：内存拷贝
来源：http://ghh.andypj.xyz

memcpy(dst, src, n);
来源：http://rnt.zhixingplan.top

[S26] C：内存清零
来源：http://zod.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://cbx.hnqzz.top

[S27] C：定义常量
来源：http://iav.zhengqikj.top

const double PI = 3.14159;
来源：http://mss.fehbvm.com

[S28] C：静态变量
来源：http://dle.tarul.cn

static int counter = 0;
来源：http://izs.xinyue.icu

[S29] C：变参函数
来源：http://pxh.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://poz.zhongyouzk.top

[S30] C：头文件保护
来源：http://cqn.zdqjudy.top

#ifndef X_H
来源：http://nzo.ivvv.top

#define X_H
来源：http://ypk.daria6918.cn

#endif
来源：http://pzh.uphjek.com

[S31] C++：Hello World
来源：http://ayr.yj20258888.top

#include <iostream>
来源：http://reg.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://gjv.ctjpmb.com

[S32] C++：字符串
来源：http://ktd.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://kxl.shzxlz.cn

[S33] C++：vector 增删
来源：http://pxq.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://evf.52xcode.cn

[S34] C++：遍历 vector
来源：http://wcr.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://kyz.shanyushiyangtech.top

[S35] C++：map
来源：http://dwi.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qqq.tian-w.cn

[S36] C++：unordered_map
来源：http://mny.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gir.wangshuangyany.cn

[S37] C++：set
来源：http://kiv.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://evh.yangfankeji.com

[S38] C++：排序
来源：http://mgr.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://xxa.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://nct.jinyuanbaomall.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ehk.zhongyouzk.top

[S40] C++：查找元素
来源：http://uzm.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cyh.jinyuanbaomall.cn


<!-- 参考信息 -->