代发 wailian999

ANALYZE TABLE users;
来源：http://qkx.yj20258.top

[Q71] 查看建表语句
来源：http://fsz.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aes.fengsongda.top

[Q72] 查看索引
来源：http://hep.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://vii.gaohongyu789.top

[Q73] 查看表状态
来源：http://bwh.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://imp.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://lyk.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gxv.shangyingyoupin.top

[Q75] 日期格式化
来源：http://osg.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qwg.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://edg.zhengqikj.top

[Q76] 按天统计
来源：http://lwe.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jbc.feifeiyinyue.top

[Q77] 时间加减
来源：http://ebt.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bcf.fehbvm.com

[Q78] 当前时间
来源：http://yzp.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mvk.haohaochexian.top

[Q79] 字符串拼接
来源：http://rkj.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kpw.cqqwz.cn

[Q80] 字符串截取
来源：http://ckb.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ggx.ydzc1.top

[Q81] 字符串替换
来源：http://oam.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kke.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://idw.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xun.gaohongyu789.top

[Q83] 大小写转换
来源：http://rxb.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pmv.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://pwb.ctjpmb.com

SELECT TRIM(name) FROM users;
来源：http://utl.tian-w.cn

[Q85] 数值取整
来源：http://ptz.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gyk.shuidangran.top

[Q86] 读取 JSON 字段
来源：http://czq.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tcd.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://uev.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vjc.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://rwa.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mko.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yzv.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://hcu.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qsk.chenzaomai.com

[Q90] 生成序号列
来源：http://yta.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://clm.yj20258.top

================================================================================
来源：http://fhj.havefunace.top

R. Bash 专题
来源：http://fum.fzhhl.top

================================================================================
来源：http://kve.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://tuw.hnqzz.top

#!/usr/bin/env bash
来源：http://usw.daxiang520.top

set -euo pipefail
来源：http://vin.yonumen.top

[R02] 变量赋值与使用
来源：http://ajl.c1oappe.top

name="Tom"; echo "$name"
来源：http://rfv.ivvv.top

[R03] 只读变量
来源：http://ppy.shanyushiyangtech.top

readonly PI=3.14
来源：http://pzv.meibo888.top

[R04] 位置参数
来源：http://cpk.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oad.ivvv.top

[R05] 参数默认值
来源：http://klj.ywan-chungtsiang.top

name="${1:-default}"
来源：http://nvr.jianghu66.top

[R06] 判断命令是否存在
来源：http://cxx.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uqx.shzxlz.cn

[R07] if 判断文件
来源：http://qau.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xkc.ivvv.top

[R08] 数值比较
来源：http://buw.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lig.zycfv.cn

[R09] 字符串比较
来源：http://dwt.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cyl.dianchejie.cn

[R10] 正则匹配
来源：http://bmg.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jct.xuanzx.com

[R11] case 多分支
来源：http://fjg.jinghuilouyu.cn

case "$1" in
来源：http://iys.shuidangran.top

start) echo "启动" ;;
来源：http://qny.shuidangran.top

stop)  echo "停止" ;;
来源：http://gti.bbcook.cn

*)     echo "未知命令" ;;
来源：http://xvo.snrcjt.cn

esac
来源：http://mpz.guannengcc.top

[R12] for 遍历文件
来源：http://cwc.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://cnk.yuxming.cn

[R13] for 计数循环
来源：http://gty.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://dso.fktsv.cn

[R14] C 风格 for
来源：http://ffd.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vfx.ctjpmb.com

[R15] while 逐行读文件
来源：http://wez.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gqj.hfpthk.cn

[R16] until 等待条件
来源：http://kun.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sov.havefunace.top

[R17] 数组定义与取值
来源：http://wha.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://pnz.uphjek.com

[R18] 遍历数组
来源：http://jkg.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vhy.c1oappe.top

[R19] 数组长度
来源：http://tat.jinqigfzy.top

echo "${#arr[@]}"
来源：http://kla.xylfe.cn

[R20] 关联数组（字典）
来源：http://pan.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eve.meibo888.top

[R21] 字符串长度
来源：http://pur.tian-w.cn

echo "${#s}"
来源：http://njl.gzhubu.top

[R22] 截取子串
来源：http://kam.redwolf501.top

echo "${s:0:5}"
来源：http://nzq.svipenyu.cn

[R23] 字符串替换
来源：http://mvy.pycfn.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aiv.pycfn.com

[R24] 大小写转换
来源：http://mrd.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://pjd.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://yao.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ydl.birdmap.top

[R26] 命令替换
来源：http://zey.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://etg.xziqi.cn

[R27] 算术展开
来源：http://tch.meibo888.top

echo $((1 + 2 * 3))
来源：http://dml.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://etl.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://xqu.hcnkem.com

[R29] 定义函数
来源：http://vcf.redwolf501.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fsk.gogol.net.cn

[R30] 函数返回状态码
来源：http://ggp.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://scf.ydzc1.top

[R31] 局部变量
来源：http://tnv.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://yzn.ehwqpu.com

[R32] 参数个数校验
来源：http://hoi.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gna.pengpengdd.cyou

[R33] 捕获错误并提示行号
来源：http://ofx.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://crx.yvedp.cn

[R34] 退出时清理
来源：http://nhl.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qvi.redwolf501.top

[R35] 后台执行并等待
来源：http://snu.ydjk.org.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wdc.c1oappe.top

[R36] 并发执行多个任务
来源：http://xiu.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://znd.yj202588.top

[R37] 把输出赋给变量
来源：http://bqt.shuidangran.top

files=$(ls -1)
来源：http://nbd.316326.xyz

[R38] 管道串联
来源：http://zoa.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://swc.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://ifh.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://awf.andypj.xyz

[R40] 追加写日志
来源：http://nho.yj20258888.top

echo "log" >> out.log
来源：http://wzb.hongshengwenyu.top

[R41] 丢弃输出
来源：http://qpz.hesvh.cn

cmd >/dev/null 2>&1
来源：http://nzd.yuanzhike.top

[R42] 输入重定向
来源：http://jjg.epnwcf.com

wc -l < a.txt
来源：http://hby.ybcxt.top

[R43] 按名字查找文件
来源：http://cka.gogol.net.cn

find . -name "*.log" -type f
来源：http://lxf.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://jkk.c1oappe.top

find . -mtime -7 -type f
来源：http://vsf.sweek.top

[R45] 批量删除
来源：http://bpt.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://lou.0kj1m.cn

[R46] 递归替换文件内容
来源：http://nej.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bnc.gzhubu.top

[R47] sed 单行替换
来源：http://pdy.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mqk.yueranfly.top

[R48] awk 取指定列
来源：http://unn.redwolf501.top

awk '{print $1, $3}' a.txt
来源：http://xqo.shuidangran.top

[R49] awk 带条件
来源：http://sqc.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nrq.chenjidiqi.icu

[R50] awk 求和
来源：http://uwi.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://kev.pycfn.com

[R51] 排序去重取前几
来源：http://dqe.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ikw.zycfv.cn

[R52] 统计行数
来源：http://myo.yfazqb.com

wc -l a.txt
来源：http://nbx.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://xph.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nzd.uphjek.com

[R54] 比较两个文件
来源：http://xjc.yuxming.cn

diff a.txt b.txt
来源：http://tbh.yfazqb.com

[R55] 压缩与解压
来源：http://kuj.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fcl.bjfxy.top

[R56] 远程拷贝
来源：http://qpx.shzxlz.cn

scp file user@host:/path/
来源：http://cup.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://bac.birdmap.top

ssh user@host 'uptime'
来源：http://joj.sufxvd.cn

[R58] 下载文件
来源：http://geu.hnqzz.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kxb.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://bbh.meibo888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rzt.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://ebm.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ovk.yueranfly.top

[R61] 磁盘占用
来源：http://ygr.zycfv.cn

df -h;  du -sh *
来源：http://gsr.birdmap.top

[R62] 找最占空间的文件
来源：http://fcn.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://zry.feifeiyinyue.top

[R63] 内存与进程
来源：http://glm.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://thl.zycfv.cn

[R64] 结束进程
来源：http://wna.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://vsz.gogol.net.cn

[R65] 查看端口占用
来源：http://dqu.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vtl.shangyingyoupin.top

[R66] 定时任务
来源：http://xft.dashuyun.cn

crontab -e;  crontab -l
来源：http://zcs.iojbl.cn

[R67] 生成随机十六进制串
来源：http://fkq.epnwcf.com

openssl rand -hex 16
来源：http://man.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://lao.guannengcc.top

sha256sum a.txt;  md5sum a.txt
来源：http://upu.mhx1999.top

[R69] 生成随机密码
来源：http://jjb.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://rag.hcnkem.com

[R70] 时间戳与互转
来源：http://msp.jyoumei.cn

date +%s;  date -d @1700000000
来源：http://jdf.guowangkeji.top

[R71] 日期格式化
来源：http://uom.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://znq.fktsv.cn

[R72] 等待端口就绪
来源：http://pqm.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jjs.zycfv.cn

[R73] 分割大日志
来源：http://ucc.sufxvd.cn

split -l 1000 big.log part_
来源：http://llt.yongpay.top

[R74] 批量重命名
来源：http://yka.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rcj.cashguo.top

[R75] 导出环境变量
来源：http://ega.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://bgh.yfazqb.com

[R76] 使用临时文件
来源：http://xnt.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zpl.fengsongda.top

[R77] 读取用户输入
来源：http://pha.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://yum.sysykeji.top

[R78] 交互式菜单
来源：http://yao.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dur.gzhubu.top

[R79] 解析命令行选项
来源：http://pgm.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xub.pycfn.com

[R80] 查看脚本执行耗时
来源：http://pnw.zycfv.cn

time ./run.sh
来源：http://hhw.tarul.cn

================================================================================
来源：http://ftq.shzxlz.cn

S. C / C++ 专题
来源：http://ymd.mhx1999.top

================================================================================
来源：http://egz.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://hnr.shanyushiyangtech.top

#include <stdio.h>
来源：http://ahc.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://prz.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://rrs.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://drw.yvedp.cn

[S03] C：读入整数
来源：http://ist.xuanzx.com

int x; scanf("%d", &x);
来源：http://ulx.yanxiufei.cn

[S04] C：字符串复制
来源：http://xuj.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://yto.xylfe.cn

[S05] C：字符串长度
来源：http://rcz.sxryk.cn

strlen(s)
来源：http://rbd.tanke756.top

[S06] C：字符串比较
来源：http://lgu.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://nec.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://uiy.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iwc.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://ayp.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tsm.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://vqe.hysaishi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dio.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://ypx.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://ynp.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://rbg.zhixingplan.top

FILE *f = fopen("a.txt", "r");
来源：http://rrq.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://pgg.wangshuangyany.cn

fclose(f);
来源：http://xdv.316326.xyz

[S12] C：写文件
来源：http://ulx.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://irr.gotoacloud.top

[S13] C：宏定义
来源：http://ncd.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yyq.yfazqb.com

[S14] C：枚举
来源：http://ltp.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://ess.sjlbkw.cn

[S15] C：类型转换
来源：http://wcu.ybcxt.top

(double) a / b
来源：http://iuq.yj20258888.top

[S16] C：位操作置位
来源：http://byi.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://ucx.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://daw.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wdk.wangshuangyany.cn

[S18] C：命令行参数
来源：http://two.tianlin.xyz

int main(int argc, char **argv)
来源：http://vnc.shzxlz.cn

[S19] C：快速排序
来源：http://yix.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://fpu.yanxiufei.cn

[S20] C：二分查找
来源：http://obz.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qli.chenzaomai.com

[S21] C：字符类别判断
来源：http://fqy.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vgi.vqdsnc.cn

[S22] C：字符串转数字
来源：http://aef.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xke.ctjpmb.com

[S23] C：随机数
来源：http://vym.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bwx.fktsv.cn

[S24] C：获取本地时间
来源：http://epe.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://syr.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://cfc.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://kfi.wangshuangyany.cn

[S26] C：内存清零
来源：http://tey.gzhubu.top

memset(a, 0, sizeof a);
来源：http://lyj.316326.xyz

[S27] C：定义常量
来源：http://hxz.zycfv.cn

const double PI = 3.14159;
来源：http://zpe.aibaodan.cn

[S28] C：静态变量
来源：http://kwx.hesvh.cn

static int counter = 0;
来源：http://duu.ehwqpu.com

[S29] C：变参函数
来源：http://vwe.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fjm.shanyushiyangtech.top

[S30] C：头文件保护
来源：http://vnz.jyoumei.cn

#ifndef X_H
来源：http://xln.chenlongwang.top

#define X_H
来源：http://vcw.yj20258888.top

#endif
来源：http://hgp.hammf.cn

[S31] C++：Hello World
来源：http://tqi.zhongyouzk.top

#include <iostream>
来源：http://yas.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://ohn.chenjidiqi.icu

[S32] C++：字符串
来源：http://ora.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://iub.nwbrower.top

[S33] C++：vector 增删
来源：http://vqi.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hsx.yvedp.cn

[S34] C++：遍历 vector
来源：http://wsk.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://mmq.cdnleiting.top

[S35] C++：map
来源：http://cxj.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kfw.xylfe.cn

[S36] C++：unordered_map
来源：http://fbs.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qsx.sjlbkw.cn

[S37] C++：set
来源：http://qex.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yro.bbcook.cn

[S38] C++：排序
来源：http://pfu.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://kfz.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://icg.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lpu.52xcode.cn

[S40] C++：查找元素
来源：http://zbm.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rcn.xuanzx.com


<!-- 参考信息 -->