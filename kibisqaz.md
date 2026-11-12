代发 wailian999

[Q67] 设置隔离级别
来源：http://emr.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uxv.hnqzz.top

[Q68] 保存点
来源：http://cmc.yuanzhike.top

SAVEPOINT sp1;
来源：http://gdh.hfpthk.cn

ROLLBACK TO sp1;
来源：http://etw.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://rfq.tarul.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://teq.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://hfl.cheryme.top

ANALYZE TABLE users;
来源：http://bze.yongpay.top

[Q71] 查看建表语句
来源：http://bwn.yuanzhike.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mph.jiagoushi.top

[Q72] 查看索引
来源：http://bgm.gotoacloud.top

SHOW INDEX FROM users;
来源：http://qof.nwbrower.top

[Q73] 查看表状态
来源：http://rra.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gdf.sweek.top

[Q74] 强制使用索引
来源：http://kqi.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ola.nwbrower.top

[Q75] 日期格式化
来源：http://jtb.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://exu.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dug.tian-w.cn

[Q76] 按天统计
来源：http://wnk.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dey.meibo888.top

[Q77] 时间加减
来源：http://akc.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tkr.jinghuilouyu.cn

[Q78] 当前时间
来源：http://rai.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ovb.316326.xyz

[Q79] 字符串拼接
来源：http://rln.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://njb.ctjpmb.com

[Q80] 字符串截取
来源：http://yem.zhijiandao.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hgb.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://qmn.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ppg.zdbjq.cn

[Q82] 字符长度与字节长度
来源：http://trj.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tdl.yvedp.cn

[Q83] 大小写转换
来源：http://nhn.jiagoushi.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tol.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://isk.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://rox.aizwys.cn

[Q85] 数值取整
来源：http://run.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yxy.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://xol.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lmy.gzhubu.top

[Q87] JSON 字段做条件
来源：http://hfq.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iqt.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://qia.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fdy.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ewa.sweek.top

[Q89] 判断表是否存在
来源：http://erj.yanxiufei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cgg.nanxuanxn.top

[Q90] 生成序号列
来源：http://lzm.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vmj.tanke756.top

================================================================================
来源：http://cpw.nanxuanxn.top

R. Bash 专题
来源：http://mgd.shzxlz.cn

================================================================================
来源：http://hoi.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://okj.fengsongda.top

#!/usr/bin/env bash
来源：http://gzx.xuetiantiany.cn

set -euo pipefail
来源：http://rnd.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://utm.dashuyun.cn

name="Tom"; echo "$name"
来源：http://poa.guannengcc.top

[R03] 只读变量
来源：http://wjs.hnxiangtu.top

readonly PI=3.14
来源：http://qzq.epnwcf.com

[R04] 位置参数
来源：http://wvh.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nbz.ybcxt.top

[R05] 参数默认值
来源：http://xhl.hcnkem.com

name="${1:-default}"
来源：http://nrz.shanyushiyangkeji.top

[R06] 判断命令是否存在
来源：http://wtp.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ugv.pengpengdd.cyou

[R07] if 判断文件
来源：http://ztq.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vvb.0kj1m.cn

[R08] 数值比较
来源：http://amg.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tbi.sysykeji.top

[R09] 字符串比较
来源：http://gsj.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zdx.smart0.xyz

[R10] 正则匹配
来源：http://gyl.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cvj.dashuyun.cn

[R11] case 多分支
来源：http://olh.ydjk.org.cn

case "$1" in
来源：http://owx.zhoulong.xyz

start) echo "启动" ;;
来源：http://gol.tanke756.top

stop)  echo "停止" ;;
来源：http://mpd.hammf.cn

*)     echo "未知命令" ;;
来源：http://dgm.zhixingplan.top

esac
来源：http://tbg.havefunace.top

[R12] for 遍历文件
来源：http://edg.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://vpe.jyoumei.cn

[R13] for 计数循环
来源：http://ojj.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://wir.daria6918.cn

[R14] C 风格 for
来源：http://red.chenjidiqi.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ymp.zycfv.cn

[R15] while 逐行读文件
来源：http://cmz.xziqi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sqf.jlsjyb.cn

[R16] until 等待条件
来源：http://hsy.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://imv.vehdjk.com

[R17] 数组定义与取值
来源：http://rhe.kuanghao11.cn

arr=(a b c); echo "${arr[0]}"
来源：http://krr.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://ifu.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://utz.cheryme.top

[R19] 数组长度
来源：http://ehi.yongpay.top

echo "${#arr[@]}"
来源：http://gmc.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://wye.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vlr.yanxiufei.cn

[R21] 字符串长度
来源：http://dqm.shanyushiyangtech.top

echo "${#s}"
来源：http://wbt.zhaomingkeji.xyz

[R22] 截取子串
来源：http://snr.tarul.cn

echo "${s:0:5}"
来源：http://eqw.chenlongwang.top

[R23] 字符串替换
来源：http://bli.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nsy.zhixingplan.top

[R24] 大小写转换
来源：http://oam.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://rcj.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://jrk.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pit.xziqi.cn

[R26] 命令替换
来源：http://anj.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://zag.haohaochexian.top

[R27] 算术展开
来源：http://fan.redwolf501.top

echo $((1 + 2 * 3))
来源：http://zia.0kj1m.cn

[R28] 浮点运算
来源：http://wxv.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://qoh.gotoacloud.top

[R29] 定义函数
来源：http://mec.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://odx.hfpthk.cn

[R30] 函数返回状态码
来源：http://epc.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://rvf.jyoumei.cn

[R31] 局部变量
来源：http://pue.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://onz.shangyingyoupin.top

[R32] 参数个数校验
来源：http://bmo.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lvd.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://dby.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yoh.hammf.cn

[R34] 退出时清理
来源：http://qbf.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://kra.vqdsnc.cn

[R35] 后台执行并等待
来源：http://wri.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uoa.zycfv.cn

[R36] 并发执行多个任务
来源：http://and.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ntg.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://lqh.shangyingyoupin.top

files=$(ls -1)
来源：http://wkk.sweek.top

[R38] 管道串联
来源：http://uwj.vqdsnc.cn

cat a.txt | grep -i error | wc -l
来源：http://wbe.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://dxw.redwolf501.top

cmd > out.log 2>&1
来源：http://zpz.sysykeji.top

[R40] 追加写日志
来源：http://ike.redwolf501.top

echo "log" >> out.log
来源：http://yiy.wangdashe.top

[R41] 丢弃输出
来源：http://bms.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://omp.jinqigufen.top

[R42] 输入重定向
来源：http://gcy.hnxiangtu.top

wc -l < a.txt
来源：http://kmq.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://cbw.haohaochexian.top

find . -name "*.log" -type f
来源：http://rlj.sysykeji.top

[R44] 按修改时间查找
来源：http://cgx.birdmap.top

find . -mtime -7 -type f
来源：http://aop.ydjk.org.cn

[R45] 批量删除
来源：http://okk.sxryk.cn

find . -name "*.tmp" -delete
来源：http://mhb.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://xdb.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://osg.fktsv.cn

[R47] sed 单行替换
来源：http://udb.nwbrower.top

sed -i 's/foo/bar/g' a.txt
来源：http://cea.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://rnj.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://spu.jqgfzy.top

[R49] awk 带条件
来源：http://suy.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fob.hesvh.cn

[R50] awk 求和
来源：http://wfg.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jnh.mhx1999.top

[R51] 排序去重取前几
来源：http://reg.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://xxi.sysykeji.top

[R52] 统计行数
来源：http://hex.zhengqikj.top

wc -l a.txt
来源：http://vey.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://gly.vehdjk.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hvd.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://uvz.chenzaomai.com

diff a.txt b.txt
来源：http://thw.cashguo.top

[R55] 压缩与解压
来源：http://uri.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://acp.epnwcf.com

[R56] 远程拷贝
来源：http://byk.hammf.cn

scp file user@host:/path/
来源：http://lxb.zhixingplan.top

[R57] 远程执行命令
来源：http://qxc.sufxvd.cn

ssh user@host 'uptime'
来源：http://vqw.chenjidiqi.icu

[R58] 下载文件
来源：http://plg.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tjx.ppjwa.cn

[R59] 发 POST JSON
来源：http://hkk.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ajk.bbcook.cn

[R60] 只看 HTTP 状态码
来源：http://vrh.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bqk.jyoumei.cn

[R61] 磁盘占用
来源：http://yks.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://qha.zycfv.cn

[R62] 找最占空间的文件
来源：http://ohm.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://wfo.wangshuangyany.cn

[R63] 内存与进程
来源：http://bmn.fengsongda.top

free -h;  ps aux | grep nginx
来源：http://nas.xylfe.cn

[R64] 结束进程
来源：http://gwx.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://jxu.nwbrower.top

[R65] 查看端口占用
来源：http://mho.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pqo.smart0.xyz

[R66] 定时任务
来源：http://izr.yvedp.cn

crontab -e;  crontab -l
来源：http://qud.c1oappe.top

[R67] 生成随机十六进制串
来源：http://lcu.gaohongyu789.top

openssl rand -hex 16
来源：http://mju.jqgufenzy.top

[R68] 计算文件校验值
来源：http://dal.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://xlg.meibo888.top

[R69] 生成随机密码
来源：http://etd.jinyuanbaomall.cn

head -c 16 /dev/urandom | base64
来源：http://gjd.52xcode.cn

[R70] 时间戳与互转
来源：http://qjt.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://iaj.bbcook.cn

[R71] 日期格式化
来源：http://ybg.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bks.havefunace.top

[R72] 等待端口就绪
来源：http://nsa.yj20258.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dtz.wangshuangyany.cn

[R73] 分割大日志
来源：http://adh.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://azk.yvedp.cn

[R74] 批量重命名
来源：http://udb.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ubc.bbcook.cn

[R75] 导出环境变量
来源：http://jvp.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://qrr.xziqi.cn

[R76] 使用临时文件
来源：http://xbt.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cdg.zycfv.cn

[R77] 读取用户输入
来源：http://scf.52xcode.cn

read -rp "请输入: " ans
来源：http://nyp.hnqzz.top

[R78] 交互式菜单
来源：http://nkc.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://zwj.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://ucl.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lvo.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://fji.zycfv.cn

time ./run.sh
来源：http://wgm.hongshengwenyu.top

================================================================================
来源：http://fiv.zhengqikj.top

S. C / C++ 专题
来源：http://lho.zhiwuduotai.top

================================================================================
来源：http://rpi.316326.xyz

[S01] C：Hello World
来源：http://xqm.aizwys.cn

#include <stdio.h>
来源：http://sia.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vrc.daria6918.cn

[S02] C：变量与格式化输出
来源：http://okh.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://zph.zhijiandao.cn

[S03] C：读入整数
来源：http://qku.sweek.top

int x; scanf("%d", &x);
来源：http://knc.hongshengwenyu.top

[S04] C：字符串复制
来源：http://qqw.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mhv.ppjwa.cn

[S05] C：字符串长度
来源：http://cby.zhixingplan.top

strlen(s)
来源：http://pjd.hysaishi.cn

[S06] C：字符串比较
来源：http://qfo.ehwqpu.com

strcmp(a, b) == 0
来源：http://ull.daxiang520.top

[S07] C：数组遍历求和
来源：http://jci.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://grs.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://yjr.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mhk.tarul.cn

[S09] C：结构体定义与初始化
来源：http://fcz.jyoumei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://poh.cqqwz.cn

[S10] C：指针与解引用
来源：http://dpy.yonumen.top

int *p = &a;  *p = 5;
来源：http://puv.hysaishi.cn

[S11] C：逐行读文件
来源：http://hoa.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://fhn.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://wyk.52xcode.cn

fclose(f);
来源：http://suf.hfpthk.cn

[S12] C：写文件
来源：http://shs.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pra.andypj.xyz

[S13] C：宏定义
来源：http://iyp.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://heg.nwbrower.top

[S14] C：枚举
来源：http://obn.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://lav.fengsongda.top

[S15] C：类型转换
来源：http://joy.uphjek.com

(double) a / b
来源：http://xsh.hywenlv.cn

[S16] C：位操作置位
来源：http://gyl.smart0.xyz

x |= (1 << 3);
来源：http://xll.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://fql.yj202588.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://itl.aibaodan.cn

[S18] C：命令行参数
来源：http://olg.jinqigufen.top

int main(int argc, char **argv)
来源：http://cwp.hnqzz.top

[S19] C：快速排序
来源：http://mwj.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://gls.yj20258888.top

[S20] C：二分查找
来源：http://xmg.dianchejie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://njt.uphjek.com

[S21] C：字符类别判断
来源：http://get.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iic.zhoulong.xyz

[S22] C：字符串转数字
来源：http://tre.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://dnl.meibo888.top

[S23] C：随机数
来源：http://rki.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yst.yueranfly.top

[S24] C：获取本地时间
来源：http://zbd.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oaj.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://hpb.wangshuangyany.cn

memcpy(dst, src, n);
来源：http://uhi.sufxvd.cn

[S26] C：内存清零
来源：http://dzx.xylfe.cn

memset(a, 0, sizeof a);
来源：http://ccy.sweek.top

[S27] C：定义常量
来源：http://izk.redwolf501.top

const double PI = 3.14159;
来源：http://csl.shuidangran.top

[S28] C：静态变量
来源：http://rdi.xingfuxueyuan.xyz

static int counter = 0;
来源：http://nnc.yangfankeji.com

[S29] C：变参函数
来源：http://xog.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://anv.birdmap.top

[S30] C：头文件保护
来源：http://kyx.hcnkem.com

#ifndef X_H
来源：http://enz.nwbrower.top

#define X_H
来源：http://kvd.ydjk.org.cn

#endif
来源：http://avw.hnqzz.top

[S31] C++：Hello World
来源：http://hrq.tianlin.xyz

#include <iostream>
来源：http://unb.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://aru.yvedp.cn

[S32] C++：字符串
来源：http://bfu.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://sxb.aizwys.cn

[S33] C++：vector 增删
来源：http://pac.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eqp.hesvh.cn

[S34] C++：遍历 vector
来源：http://atb.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://isx.zhixingplan.top

[S35] C++：map
来源：http://iro.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ypm.pycfn.com

[S36] C++：unordered_map
来源：http://elr.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jpz.ctjpmb.com


<!-- 参考信息 -->