代发 wailian999

[Q67] 设置隔离级别
来源：http://nty.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bgy.sufxvd.cn

[Q68] 保存点
来源：http://dnx.yj20258.top

SAVEPOINT sp1;
来源：http://kwg.uphjek.com

ROLLBACK TO sp1;
来源：http://wbt.daxiang520.top

[Q69] 查看执行计划
来源：http://cmu.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://npn.zdqjudy.top

[Q70] 更新统计信息
来源：http://obw.gogol.net.cn

ANALYZE TABLE users;
来源：http://mbn.pycfn.com

[Q71] 查看建表语句
来源：http://sho.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yqw.jinqigfzy.top

[Q72] 查看索引
来源：http://ith.cashguo.top

SHOW INDEX FROM users;
来源：http://igx.uphjek.com

[Q73] 查看表状态
来源：http://eul.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://oeb.gaohongyu789.top

[Q74] 强制使用索引
来源：http://hfb.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wec.cheryme.top

[Q75] 日期格式化
来源：http://tzi.mhx1999.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://udy.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yeg.nanxuanxn.top

[Q76] 按天统计
来源：http://ofv.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xnf.ydjk.org.cn

[Q77] 时间加减
来源：http://ajd.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://upd.aibaodan.cn

[Q78] 当前时间
来源：http://ivq.sysykeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xfd.svipenyu.cn

[Q79] 字符串拼接
来源：http://vfa.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bno.pycfn.com

[Q80] 字符串截取
来源：http://qei.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rkq.daria6918.cn

[Q81] 字符串替换
来源：http://kai.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eqx.sxryk.cn

[Q82] 字符长度与字节长度
来源：http://ncz.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ybb.jlsjyb.cn

[Q83] 大小写转换
来源：http://ngf.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qye.vehdjk.com

[Q84] 去除首尾空格
来源：http://wzb.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://zod.yj20258.top

[Q85] 数值取整
来源：http://aad.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jos.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://nxu.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ikx.hfpthk.cn

[Q87] JSON 字段做条件
来源：http://gtj.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hpm.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://kvd.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bdv.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jvb.cqqwz.cn

[Q89] 判断表是否存在
来源：http://dgv.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xic.vehdjk.com

[Q90] 生成序号列
来源：http://zcc.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xwx.zhiwuduotai.top

================================================================================
来源：http://mjm.bbcook.cn

R. Bash 专题
来源：http://dcp.jqgfzy.top

================================================================================
来源：http://ycn.shzxlz.cn

[R01] shebang 与严格模式
来源：http://eqn.yangfankeji.com

#!/usr/bin/env bash
来源：http://cid.tanke756.top

set -euo pipefail
来源：http://mqz.ybcxt.top

[R02] 变量赋值与使用
来源：http://chg.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://vgo.yongpay.top

[R03] 只读变量
来源：http://jgn.hammf.cn

readonly PI=3.14
来源：http://cmz.ppjwa.cn

[R04] 位置参数
来源：http://ilt.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oia.bjfxy.top

[R05] 参数默认值
来源：http://bhw.0kj1m.cn

name="${1:-default}"
来源：http://pvp.sweek.top

[R06] 判断命令是否存在
来源：http://iaq.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iud.cheryme.top

[R07] if 判断文件
来源：http://fkp.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ajn.wangshuangyany.cn

[R08] 数值比较
来源：http://pun.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dsw.ehwqpu.com

[R09] 字符串比较
来源：http://mbz.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rxx.9152youxi.cn

[R10] 正则匹配
来源：http://ipx.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xyp.shangyingyoupin.top

[R11] case 多分支
来源：http://fqx.wangshuangyany.cn

case "$1" in
来源：http://wbe.tianlin.xyz

start) echo "启动" ;;
来源：http://dvh.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://mwi.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://nus.snrcjt.cn

esac
来源：http://yvw.wangdashe.top

[R12] for 遍历文件
来源：http://pby.xziqi.cn

for f in *.txt; do echo "$f"; done
来源：http://fvp.chenjidiqi.icu

[R13] for 计数循环
来源：http://ues.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://flq.0kj1m.cn

[R14] C 风格 for
来源：http://fyc.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ytj.cqqwz.cn

[R15] while 逐行读文件
来源：http://zri.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://onv.fzhhl.top

[R16] until 等待条件
来源：http://fbh.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xrz.yangfankeji.com

[R17] 数组定义与取值
来源：http://pqx.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://okm.9152youxi.cn

[R18] 遍历数组
来源：http://qgs.sufxvd.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wnc.zhongyouzk.top

[R19] 数组长度
来源：http://ggx.ybcxt.top

echo "${#arr[@]}"
来源：http://zba.gogol.net.cn

[R20] 关联数组（字典）
来源：http://adn.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xsj.bbcook.cn

[R21] 字符串长度
来源：http://mkc.ehwqpu.com

echo "${#s}"
来源：http://ipa.pycfn.com

[R22] 截取子串
来源：http://twi.yj20258.top

echo "${s:0:5}"
来源：http://buo.yuanzhike.top

[R23] 字符串替换
来源：http://yxa.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jxc.daria6918.cn

[R24] 大小写转换
来源：http://wyb.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qye.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://lzr.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://txp.yueranfly.top

[R26] 命令替换
来源：http://yxp.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://hte.smart0.xyz

[R27] 算术展开
来源：http://izq.quarkkingdee.top

echo $((1 + 2 * 3))
来源：http://yee.quarkkingdee.top

[R28] 浮点运算
来源：http://bwt.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://flw.mhx1999.top

[R29] 定义函数
来源：http://okp.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bol.bjfxy.top

[R30] 函数返回状态码
来源：http://nba.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://pyn.vehdjk.com

[R31] 局部变量
来源：http://iei.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://ttk.yueranfly.top

[R32] 参数个数校验
来源：http://blw.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zaz.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://uii.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sxx.yj20258888.top

[R34] 退出时清理
来源：http://zbn.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://frg.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://obe.aibaodan.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bxu.yuxming.cn

[R36] 并发执行多个任务
来源：http://quc.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dbf.jqgfzy.top

[R37] 把输出赋给变量
来源：http://kga.jyoumei.cn

files=$(ls -1)
来源：http://bgq.zdqjudy.top

[R38] 管道串联
来源：http://puv.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://jzo.9152youxi.cn

[R39] 重定向标准输出与错误
来源：http://kni.shuidangran.top

cmd > out.log 2>&1
来源：http://bht.ehwqpu.com

[R40] 追加写日志
来源：http://ebi.daria6918.cn

echo "log" >> out.log
来源：http://jeu.xylfe.cn

[R41] 丢弃输出
来源：http://sqc.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://djb.jlsjyb.cn

[R42] 输入重定向
来源：http://hff.xinyue.icu

wc -l < a.txt
来源：http://vmp.jyoumei.cn

[R43] 按名字查找文件
来源：http://ugr.yfazqb.com

find . -name "*.log" -type f
来源：http://bci.chenzaomai.com

[R44] 按修改时间查找
来源：http://inx.316326.xyz

find . -mtime -7 -type f
来源：http://oya.hysaishi.cn

[R45] 批量删除
来源：http://mxz.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://izz.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://mlm.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kuw.zhengqikj.top

[R47] sed 单行替换
来源：http://lok.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://gmm.hammf.cn

[R48] awk 取指定列
来源：http://onu.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://ihg.9152youxi.cn

[R49] awk 带条件
来源：http://fow.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gsz.cheryme.top

[R50] awk 求和
来源：http://prl.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cuj.yj20258888.top

[R51] 排序去重取前几
来源：http://cpu.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://btf.xylfe.cn

[R52] 统计行数
来源：http://tmm.yongpay.top

wc -l a.txt
来源：http://hjr.havefunace.top

[R53] 查看文件头与实时尾
来源：http://ggx.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fiu.xuetiantiany.cn

[R54] 比较两个文件
来源：http://bck.nanxinkj.top

diff a.txt b.txt
来源：http://qbo.uphjek.com

[R55] 压缩与解压
来源：http://sac.yfazqb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bls.zhijiandao.cn

[R56] 远程拷贝
来源：http://jsy.yj20258888.top

scp file user@host:/path/
来源：http://qpq.zhijiandao.cn

[R57] 远程执行命令
来源：http://yjz.jinqigfzy.top

ssh user@host 'uptime'
来源：http://ztj.zhaomingkeji.xyz

[R58] 下载文件
来源：http://bsa.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wyu.52xcode.cn

[R59] 发 POST JSON
来源：http://zss.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://euw.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://zpm.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ehq.hammf.cn

[R61] 磁盘占用
来源：http://vmj.bbcook.cn

df -h;  du -sh *
来源：http://bfh.cucudq.cn

[R62] 找最占空间的文件
来源：http://xvx.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://uuu.svipenyu.cn

[R63] 内存与进程
来源：http://doz.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://evg.sysykeji.top

[R64] 结束进程
来源：http://koi.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://rtn.52xcode.cn

[R65] 查看端口占用
来源：http://kqo.yj20258.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ujf.yfazqb.com

[R66] 定时任务
来源：http://jwp.sysykeji.top

crontab -e;  crontab -l
来源：http://gpl.zhoulong.xyz

[R67] 生成随机十六进制串
来源：http://azv.fzhhl.top

openssl rand -hex 16
来源：http://dbz.yueranfly.top

[R68] 计算文件校验值
来源：http://lvl.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://yzz.c1oappe.top

[R69] 生成随机密码
来源：http://knd.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://efr.kuanghao11.cn

[R70] 时间戳与互转
来源：http://aem.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://fwk.bbcook.cn

[R71] 日期格式化
来源：http://dxe.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bsj.andypj.xyz

[R72] 等待端口就绪
来源：http://xio.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://zir.quarkkingdee.top

[R73] 分割大日志
来源：http://vlf.xylfe.cn

split -l 1000 big.log part_
来源：http://tje.hnqzz.top

[R74] 批量重命名
来源：http://ddo.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xzr.ybcxt.top

[R75] 导出环境变量
来源：http://ijw.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://cce.bbcook.cn

[R76] 使用临时文件
来源：http://fdv.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fyt.yongpay.top

[R77] 读取用户输入
来源：http://tra.cheryme.top

read -rp "请输入: " ans
来源：http://jfh.jinqigfzy.top

[R78] 交互式菜单
来源：http://iri.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jhr.jinqigfzy.top

[R79] 解析命令行选项
来源：http://nwt.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://szs.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://ysb.gotoacloud.top

time ./run.sh
来源：http://fik.nwbrower.top

================================================================================
来源：http://wgq.sufxvd.cn

S. C / C++ 专题
来源：http://ytw.yuanzhike.top

================================================================================
来源：http://ylx.tarul.cn

[S01] C：Hello World
来源：http://mrm.zdbjq.cn

#include <stdio.h>
来源：http://lsn.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://vuy.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://zeh.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://ixa.chenzaomai.com

[S03] C：读入整数
来源：http://cep.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://elw.zhongyouzk.top

[S04] C：字符串复制
来源：http://fme.sxryk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ndg.xziqi.cn

[S05] C：字符串长度
来源：http://sfk.svipenyu.cn

strlen(s)
来源：http://eit.hysaishi.cn

[S06] C：字符串比较
来源：http://gno.zhijiandao.cn

strcmp(a, b) == 0
来源：http://mkl.dashuyun.cn

[S07] C：数组遍历求和
来源：http://ztl.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ywv.yj20258.top

[S08] C：动态内存分配与释放
来源：http://lpc.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qia.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://ypt.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uuh.jqgufenzy.top

[S10] C：指针与解引用
来源：http://mph.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://agh.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://mve.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://asd.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://edi.dianchejie.cn

fclose(f);
来源：http://iyr.meibo888.top

[S12] C：写文件
来源：http://kcv.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jkb.gaohongyu789.top

[S13] C：宏定义
来源：http://fuj.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://flo.shanyushiyangtech.top

[S14] C：枚举
来源：http://wlm.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://psb.0kj1m.cn

[S15] C：类型转换
来源：http://awp.smart0.xyz

(double) a / b
来源：http://tqx.yangfankeji.com

[S16] C：位操作置位
来源：http://vgg.sufxvd.cn

x |= (1 << 3);
来源：http://heg.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://yay.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cuf.0kj1m.cn

[S18] C：命令行参数
来源：http://qaa.jinghuilouyu.cn

int main(int argc, char **argv)
来源：http://wio.sufxvd.cn

[S19] C：快速排序
来源：http://dxx.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://ahu.svipenyu.cn

[S20] C：二分查找
来源：http://jec.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zph.yvedp.cn

[S21] C：字符类别判断
来源：http://kid.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qrj.nanxinkj.top

[S22] C：字符串转数字
来源：http://moc.gaohongyu789.top

atoi("42");  strtod("3.14", NULL);
来源：http://qkv.zdqjudy.top

[S23] C：随机数
来源：http://iip.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bcn.ctjpmb.com

[S24] C：获取本地时间
来源：http://zqk.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gxs.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://khq.kuanghao11.cn

memcpy(dst, src, n);
来源：http://slm.jlsjyb.cn

[S26] C：内存清零
来源：http://tly.cashguo.top

memset(a, 0, sizeof a);
来源：http://wuk.yvedp.cn

[S27] C：定义常量
来源：http://whg.nanxuanxn.top

const double PI = 3.14159;
来源：http://qlm.dianchejie.cn

[S28] C：静态变量
来源：http://zns.aibaodan.cn

static int counter = 0;
来源：http://eim.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://ica.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://efu.9152youxi.cn

[S30] C：头文件保护
来源：http://ymi.iojbl.cn

#ifndef X_H
来源：http://eoi.yfazqb.com

#define X_H
来源：http://pef.kuanghao11.cn

#endif
来源：http://jbg.hnqzz.top

[S31] C++：Hello World
来源：http://age.yuxming.cn

#include <iostream>
来源：http://weg.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://imw.cheryme.top

[S32] C++：字符串
来源：http://pbm.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://jaw.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://wti.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ask.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://qdq.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://aov.tanke756.top

[S35] C++：map
来源：http://zvz.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://caf.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://epl.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wnr.ybcxt.top


<!-- 参考信息 -->