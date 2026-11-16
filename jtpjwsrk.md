代发 wailian999

ROLLBACK TO sp1;
来源：http://dgt.aizwys.cn

[Q69] 查看执行计划
来源：http://rti.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pcm.cqqwz.cn

[Q70] 更新统计信息
来源：http://zzh.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://fkm.jyoumei.cn

[Q71] 查看建表语句
来源：http://cec.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lhz.uphjek.com

[Q72] 查看索引
来源：http://tdn.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://emz.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://jix.pycfn.com

SHOW TABLE STATUS LIKE 'users';
来源：http://kga.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://vio.cheryme.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qqj.gogol.net.cn

[Q75] 日期格式化
来源：http://dxk.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wjr.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pro.hfpthk.cn

[Q76] 按天统计
来源：http://gke.jinyuanbaomall.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mlj.nwbrower.top

[Q77] 时间加减
来源：http://pat.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://osi.vehdjk.com

[Q78] 当前时间
来源：http://rrc.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bpg.gogol.net.cn

[Q79] 字符串拼接
来源：http://bbl.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dkd.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://fcn.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hag.tianlin.xyz

[Q81] 字符串替换
来源：http://qng.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fzw.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://gyf.nwbrower.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ivo.316326.xyz

[Q83] 大小写转换
来源：http://hvk.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lie.zhengqikj.top

[Q84] 去除首尾空格
来源：http://ntz.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://xqz.9152youxi.cn

[Q85] 数值取整
来源：http://xtq.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mbo.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://cly.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ila.wangdashe.top

[Q87] JSON 字段做条件
来源：http://kod.wangshuangyany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qtr.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://eom.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nsh.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lek.jyoumei.cn

[Q89] 判断表是否存在
来源：http://lvq.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yxc.ctjpmb.com

[Q90] 生成序号列
来源：http://qpu.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mzc.zhixingplan.top

================================================================================
来源：http://vuz.ivvv.top

R. Bash 专题
来源：http://ptq.guannengcc.top

================================================================================
来源：http://wop.fehbvm.com

[R01] shebang 与严格模式
来源：http://ggc.epnwcf.com

#!/usr/bin/env bash
来源：http://fwd.dianchejie.cn

set -euo pipefail
来源：http://wgs.0kj1m.cn

[R02] 变量赋值与使用
来源：http://xjs.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://ypd.birdmap.top

[R03] 只读变量
来源：http://osb.epnwcf.com

readonly PI=3.14
来源：http://elo.xuanzx.com

[R04] 位置参数
来源：http://fec.jianghu66.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ecg.guannengcc.top

[R05] 参数默认值
来源：http://kqr.sufxvd.cn

name="${1:-default}"
来源：http://olv.zhengqikj.top

[R06] 判断命令是否存在
来源：http://xtx.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zrs.cqqwz.cn

[R07] if 判断文件
来源：http://smf.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://grz.zdbjq.cn

[R08] 数值比较
来源：http://nir.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sru.jinghuilouyu.cn

[R09] 字符串比较
来源：http://pkn.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://itm.nwbrower.top

[R10] 正则匹配
来源：http://wuk.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uwx.sjlbkw.cn

[R11] case 多分支
来源：http://cna.yongpay.top

case "$1" in
来源：http://tdg.nanxinkj.top

start) echo "启动" ;;
来源：http://xlc.shzxlz.cn

stop)  echo "停止" ;;
来源：http://ltw.yuxming.cn

*)     echo "未知命令" ;;
来源：http://dqe.guowangkeji.top

esac
来源：http://phf.zhixingplan.top

[R12] for 遍历文件
来源：http://ugc.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://wow.vqdsnc.cn

[R13] for 计数循环
来源：http://oqx.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://ldk.zdbjq.cn

[R14] C 风格 for
来源：http://asy.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eel.cdnleiting.top

[R15] while 逐行读文件
来源：http://qmw.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://brz.havefunace.top

[R16] until 等待条件
来源：http://klu.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kza.gzhubu.top

[R17] 数组定义与取值
来源：http://krw.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://ygf.bbcook.cn

[R18] 遍历数组
来源：http://fpm.xinyue.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kwg.jyoumei.cn

[R19] 数组长度
来源：http://ldd.uphjek.com

echo "${#arr[@]}"
来源：http://vmg.hcnkem.com

[R20] 关联数组（字典）
来源：http://abz.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qch.haohaochexian.top

[R21] 字符串长度
来源：http://psb.0kj1m.cn

echo "${#s}"
来源：http://vvd.mhx1999.top

[R22] 截取子串
来源：http://qug.sufxvd.cn

echo "${s:0:5}"
来源：http://hys.hfpthk.cn

[R23] 字符串替换
来源：http://wyl.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sav.xuanzx.com

[R24] 大小写转换
来源：http://qkj.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://nay.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://kap.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gfq.havefunace.top

[R26] 命令替换
来源：http://euq.yonumen.top

now=$(date +%F); echo "$now"
来源：http://vae.hnxiangtu.top

[R27] 算术展开
来源：http://yff.pycfn.com

echo $((1 + 2 * 3))
来源：http://rvq.birdmap.top

[R28] 浮点运算
来源：http://vuh.uphjek.com

echo "scale=2; 10/3" | bc
来源：http://bsu.zhixingplan.top

[R29] 定义函数
来源：http://lug.xingfuxueyuan.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ibv.fengsongda.top

[R30] 函数返回状态码
来源：http://tyj.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://ppx.yuanzhike.top

[R31] 局部变量
来源：http://vbc.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://xkz.yanxiufei.cn

[R32] 参数个数校验
来源：http://jst.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wew.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://hxx.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iyc.svipenyu.cn

[R34] 退出时清理
来源：http://pol.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://ogq.cucudq.cn

[R35] 后台执行并等待
来源：http://diw.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xiv.0kj1m.cn

[R36] 并发执行多个任务
来源：http://ywu.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zhy.ppjwa.cn

[R37] 把输出赋给变量
来源：http://mgy.zhiwuduotai.top

files=$(ls -1)
来源：http://zmq.hfpthk.cn

[R38] 管道串联
来源：http://bwc.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://lzr.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://wfw.ctjpmb.com

cmd > out.log 2>&1
来源：http://xkd.shangyingyoupin.top

[R40] 追加写日志
来源：http://rmv.guowangkeji.top

echo "log" >> out.log
来源：http://arn.uphjek.com

[R41] 丢弃输出
来源：http://bld.yj20258.top

cmd >/dev/null 2>&1
来源：http://rkz.sweek.top

[R42] 输入重定向
来源：http://pva.yfazqb.com

wc -l < a.txt
来源：http://ptp.shzxlz.cn

[R43] 按名字查找文件
来源：http://yhj.bjfxy.top

find . -name "*.log" -type f
来源：http://vio.yangfankeji.com

[R44] 按修改时间查找
来源：http://juv.aizwys.cn

find . -mtime -7 -type f
来源：http://yhw.xinyue.icu

[R45] 批量删除
来源：http://ajr.tanke756.top

find . -name "*.tmp" -delete
来源：http://jmk.yfazqb.com

[R46] 递归替换文件内容
来源：http://cai.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zcq.fehbvm.com

[R47] sed 单行替换
来源：http://wlh.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://pwv.zhongyouzk.top

[R48] awk 取指定列
来源：http://oxa.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://ofv.wangdashe.top

[R49] awk 带条件
来源：http://mmc.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qep.tanke756.top

[R50] awk 求和
来源：http://aut.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://lip.chenzaomai.com

[R51] 排序去重取前几
来源：http://gxd.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://irf.xylfe.cn

[R52] 统计行数
来源：http://dex.xinyue.icu

wc -l a.txt
来源：http://woa.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://zte.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://opm.aibaodan.cn

[R54] 比较两个文件
来源：http://jbk.iojbl.cn

diff a.txt b.txt
来源：http://kpo.shuidangran.top

[R55] 压缩与解压
来源：http://lhc.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uid.nwbrower.top

[R56] 远程拷贝
来源：http://qec.meibo888.top

scp file user@host:/path/
来源：http://uzk.bjfxy.top

[R57] 远程执行命令
来源：http://uxq.0kj1m.cn

ssh user@host 'uptime'
来源：http://qrg.zhengqikj.top

[R58] 下载文件
来源：http://mil.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sly.yangfankeji.com

[R59] 发 POST JSON
来源：http://gwo.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dgd.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://upr.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lhe.ybcxt.top

[R61] 磁盘占用
来源：http://dtt.meibo888.top

df -h;  du -sh *
来源：http://jlg.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://ivz.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://ida.aibaodan.cn

[R63] 内存与进程
来源：http://fxa.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://yuj.ydjk.org.cn

[R64] 结束进程
来源：http://spd.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://fpr.zhengqikj.top

[R65] 查看端口占用
来源：http://mkt.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kho.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://ori.sufxvd.cn

crontab -e;  crontab -l
来源：http://wcz.cheryme.top

[R67] 生成随机十六进制串
来源：http://bpg.ydzc1.top

openssl rand -hex 16
来源：http://yyg.dianchejie.cn

[R68] 计算文件校验值
来源：http://uir.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://igp.zhijiandao.cn

[R69] 生成随机密码
来源：http://eic.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://gly.yj20258888.top

[R70] 时间戳与互转
来源：http://guv.hnqzz.top

date +%s;  date -d @1700000000
来源：http://nym.sweek.top

[R71] 日期格式化
来源：http://luu.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hde.zhoulong.xyz

[R72] 等待端口就绪
来源：http://xsq.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://qaa.svipenyu.cn

[R73] 分割大日志
来源：http://vzg.kuanghao11.cn

split -l 1000 big.log part_
来源：http://dpo.yfazqb.com

[R74] 批量重命名
来源：http://hdm.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iym.sweek.top

[R75] 导出环境变量
来源：http://hjy.jqgufenzy.top

export PATH="$HOME/bin:$PATH"
来源：http://azu.c1oappe.top

[R76] 使用临时文件
来源：http://poa.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hxu.yj20258.top

[R77] 读取用户输入
来源：http://sjl.yongpay.top

read -rp "请输入: " ans
来源：http://umn.tian-w.cn

[R78] 交互式菜单
来源：http://lwa.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ttw.yuxming.cn

[R79] 解析命令行选项
来源：http://hno.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://voz.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://lwg.zdbjq.cn

time ./run.sh
来源：http://qvz.yanxiufei.cn

================================================================================
来源：http://wub.zycfv.cn

S. C / C++ 专题
来源：http://xky.kuanghao11.cn

================================================================================
来源：http://jfr.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://klx.meibo888.top

#include <stdio.h>
来源：http://rrn.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://pxu.wangdashe.top

[S02] C：变量与格式化输出
来源：http://otd.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://fhz.pengpengdd.cyou

[S03] C：读入整数
来源：http://oqu.hywenlv.cn

int x; scanf("%d", &x);
来源：http://kta.dianchejie.cn

[S04] C：字符串复制
来源：http://fjq.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ily.fengsongda.top

[S05] C：字符串长度
来源：http://kky.mhx1999.top

strlen(s)
来源：http://ame.sjlbkw.cn

[S06] C：字符串比较
来源：http://lcr.havefunace.top

strcmp(a, b) == 0
来源：http://rvs.yj202588.top

[S07] C：数组遍历求和
来源：http://epe.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://izf.havefunace.top

[S08] C：动态内存分配与释放
来源：http://met.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yoj.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://azv.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://knc.daxiang520.top

[S10] C：指针与解引用
来源：http://qeu.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://agu.c1oappe.top

[S11] C：逐行读文件
来源：http://gbs.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://swt.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hgy.0kj1m.cn

fclose(f);
来源：http://hzf.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://wsx.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rri.pengpengdd.cyou

[S13] C：宏定义
来源：http://gca.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ssr.hywenlv.cn

[S14] C：枚举
来源：http://cbv.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://ftf.epnwcf.com

[S15] C：类型转换
来源：http://dyt.andypj.xyz

(double) a / b
来源：http://ukq.sjlbkw.cn

[S16] C：位操作置位
来源：http://biy.uphjek.com

x |= (1 << 3);
来源：http://fcu.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://cbs.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://epa.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://qss.shzxlz.cn

int main(int argc, char **argv)
来源：http://qed.hnxiangtu.top

[S19] C：快速排序
来源：http://gxx.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ono.tian-w.cn

[S20] C：二分查找
来源：http://usn.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nts.fzhhl.top

[S21] C：字符类别判断
来源：http://xjm.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uvs.cheryme.top

[S22] C：字符串转数字
来源：http://hum.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://cnu.uphjek.com

[S23] C：随机数
来源：http://kgh.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://rfw.yanxiufei.cn

[S24] C：获取本地时间
来源：http://wbq.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xep.dianchejie.cn

[S25] C：内存拷贝
来源：http://dze.sysykeji.top

memcpy(dst, src, n);
来源：http://rol.52xcode.cn

[S26] C：内存清零
来源：http://rfk.c1oappe.top

memset(a, 0, sizeof a);
来源：http://yos.yuanzhike.top

[S27] C：定义常量
来源：http://btg.hammf.cn

const double PI = 3.14159;
来源：http://lsh.xuanzx.com

[S28] C：静态变量
来源：http://xll.mhx1999.top

static int counter = 0;
来源：http://awr.zdqjudy.top

[S29] C：变参函数
来源：http://tct.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zke.mhx1999.top

[S30] C：头文件保护
来源：http://dyx.zhaomingkeji.xyz

#ifndef X_H
来源：http://won.pengpengdd.cyou

#define X_H
来源：http://cxj.zycfv.cn

#endif
来源：http://twh.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://aih.hesvh.cn

#include <iostream>
来源：http://aih.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://dlw.fengsongda.top

[S32] C++：字符串
来源：http://gfw.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://ipg.chenlongwang.top

[S33] C++：vector 增删
来源：http://yiw.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jeq.svipenyu.cn

[S34] C++：遍历 vector
来源：http://jft.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://pgg.hongshengwenyu.top

[S35] C++：map
来源：http://blz.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://noh.52xcode.cn

[S36] C++：unordered_map
来源：http://ije.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fqy.ydjk.org.cn

[S37] C++：set
来源：http://ejy.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wbc.jqgufenzy.top

[S38] C++：排序
来源：http://iiz.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://pnc.shuidangran.top


<!-- 参考信息 -->