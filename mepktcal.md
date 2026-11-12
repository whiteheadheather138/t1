代发 wailian999

[Q65] 回滚事务
来源：http://feg.jyoumei.cn

ROLLBACK;
来源：http://kfg.aibaodan.cn

[Q66] 行锁查询
来源：http://lcb.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tzv.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://yvw.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://efi.316326.xyz

[Q68] 保存点
来源：http://guc.gotoacloud.top

SAVEPOINT sp1;
来源：http://sri.ydzc1.top

ROLLBACK TO sp1;
来源：http://qiq.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://fbg.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ghc.sjlbkw.cn

[Q70] 更新统计信息
来源：http://fez.ppjwa.cn

ANALYZE TABLE users;
来源：http://mfv.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://vvp.yuanzhike.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fae.yvedp.cn

[Q72] 查看索引
来源：http://ett.jqgfzy.top

SHOW INDEX FROM users;
来源：http://flu.dianchejie.cn

[Q73] 查看表状态
来源：http://lew.guannengcc.top

SHOW TABLE STATUS LIKE 'users';
来源：http://taz.tanke756.top

[Q74] 强制使用索引
来源：http://hcw.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jwf.fktsv.cn

[Q75] 日期格式化
来源：http://dbn.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ikm.jqgufenzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dox.zdqjudy.top

[Q76] 按天统计
来源：http://jeg.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yfs.nwbrower.top

[Q77] 时间加减
来源：http://tst.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mqi.jianghu66.top

[Q78] 当前时间
来源：http://awm.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fla.jinqigfzy.top

[Q79] 字符串拼接
来源：http://vlj.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ujx.fanxiaobao.xyz

[Q80] 字符串截取
来源：http://pqf.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ghb.smart0.xyz

[Q81] 字符串替换
来源：http://vnm.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kvy.svipenyu.cn

[Q82] 字符长度与字节长度
来源：http://lbd.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uma.feifeiyinyue.top

[Q83] 大小写转换
来源：http://jzq.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qpj.yfazqb.com

[Q84] 去除首尾空格
来源：http://xrq.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://dkm.feifeiyinyue.top

[Q85] 数值取整
来源：http://iln.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://isw.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://sga.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://azz.fengsongda.top

[Q87] JSON 字段做条件
来源：http://bit.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ucj.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://mfo.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cla.svipenyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://twm.jqgfzy.top

[Q89] 判断表是否存在
来源：http://fck.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dql.aibaodan.cn

[Q90] 生成序号列
来源：http://uqp.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mlm.zhengqikj.top

================================================================================
来源：http://unq.tianlin.xyz

R. Bash 专题
来源：http://dtu.c1oappe.top

================================================================================
来源：http://eft.uphjek.com

[R01] shebang 与严格模式
来源：http://nhk.chenzaomai.com

#!/usr/bin/env bash
来源：http://etw.yfazqb.com

set -euo pipefail
来源：http://ijn.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://mof.bjfxy.top

name="Tom"; echo "$name"
来源：http://yok.cheryme.top

[R03] 只读变量
来源：http://oco.yfazqb.com

readonly PI=3.14
来源：http://wrb.chenlongwang.top

[R04] 位置参数
来源：http://xsl.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pmw.andypj.xyz

[R05] 参数默认值
来源：http://ugf.hfpthk.cn

name="${1:-default}"
来源：http://qai.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://ofm.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mtg.cheryme.top

[R07] if 判断文件
来源：http://ddc.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wyk.meibo888.top

[R08] 数值比较
来源：http://glr.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://htt.tanke756.top

[R09] 字符串比较
来源：http://mdd.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qip.ydzc1.top

[R10] 正则匹配
来源：http://bpy.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ylp.zhijiandao.cn

[R11] case 多分支
来源：http://kmz.zhaomingkeji.xyz

case "$1" in
来源：http://smz.ydjk.org.cn

start) echo "启动" ;;
来源：http://apn.tarul.cn

stop)  echo "停止" ;;
来源：http://ree.cashguo.top

*)     echo "未知命令" ;;
来源：http://pyg.fehbvm.com

esac
来源：http://fge.cucudq.cn

[R12] for 遍历文件
来源：http://rjl.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://gtd.yvedp.cn

[R13] for 计数循环
来源：http://wpg.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://ioh.zhixingplan.top

[R14] C 风格 for
来源：http://zga.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://znn.jianghu66.top

[R15] while 逐行读文件
来源：http://kph.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jjb.jinqigfzy.top

[R16] until 等待条件
来源：http://xvx.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uwm.zycfv.cn

[R17] 数组定义与取值
来源：http://quh.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pav.hysaishi.cn

[R18] 遍历数组
来源：http://haz.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aoc.gaohongyu789.top

[R19] 数组长度
来源：http://dfx.gzhubu.top

echo "${#arr[@]}"
来源：http://hzu.nwbrower.top

[R20] 关联数组（字典）
来源：http://lsn.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cdi.hfpthk.cn

[R21] 字符串长度
来源：http://djc.gogol.net.cn

echo "${#s}"
来源：http://eyu.iojbl.cn

[R22] 截取子串
来源：http://igk.zhengqikj.top

echo "${s:0:5}"
来源：http://pyf.shzxlz.cn

[R23] 字符串替换
来源：http://ulb.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jsc.sjlbkw.cn

[R24] 大小写转换
来源：http://ubb.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://wdx.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://fsb.iojbl.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oha.jianghu66.top

[R26] 命令替换
来源：http://ugk.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://kft.sufxvd.cn

[R27] 算术展开
来源：http://xpi.yj202588.top

echo $((1 + 2 * 3))
来源：http://sqm.yangfankeji.com

[R28] 浮点运算
来源：http://wng.uphjek.com

echo "scale=2; 10/3" | bc
来源：http://url.yanxiufei.cn

[R29] 定义函数
来源：http://gyx.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iik.9152youxi.cn

[R30] 函数返回状态码
来源：http://fci.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://dxb.ybcxt.top

[R31] 局部变量
来源：http://cuw.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://mfx.jinqigfzy.top

[R32] 参数个数校验
来源：http://thr.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://shi.yj202588.top

[R33] 捕获错误并提示行号
来源：http://kfu.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gjc.xziqi.cn

[R34] 退出时清理
来源：http://zdq.316326.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ydc.bbcook.cn

[R35] 后台执行并等待
来源：http://vre.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jjr.cdnleiting.top

[R36] 并发执行多个任务
来源：http://sct.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hil.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://rtz.vehdjk.com

files=$(ls -1)
来源：http://rsf.yfazqb.com

[R38] 管道串联
来源：http://xtf.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://tmb.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://cxh.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://ngc.gotoacloud.top

[R40] 追加写日志
来源：http://mvm.yj202588.top

echo "log" >> out.log
来源：http://nil.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://ncp.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://bvd.hesvh.cn

[R42] 输入重定向
来源：http://lem.cucudq.cn

wc -l < a.txt
来源：http://vkf.chenlongwang.top

[R43] 按名字查找文件
来源：http://sgg.uphjek.com

find . -name "*.log" -type f
来源：http://thn.jianghu66.top

[R44] 按修改时间查找
来源：http://kry.zhiwuduotai.top

find . -mtime -7 -type f
来源：http://dgv.xziqi.cn

[R45] 批量删除
来源：http://plv.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://hei.tianlin.xyz

[R46] 递归替换文件内容
来源：http://irh.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lzu.andypj.xyz

[R47] sed 单行替换
来源：http://zsw.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ekn.yonumen.top

[R48] awk 取指定列
来源：http://hzo.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://sxr.jyoumei.cn

[R49] awk 带条件
来源：http://qwq.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jly.gzhubu.top

[R50] awk 求和
来源：http://tvf.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://yad.hammf.cn

[R51] 排序去重取前几
来源：http://czy.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gob.zdqjudy.top

[R52] 统计行数
来源：http://bqp.jinqigfzy.top

wc -l a.txt
来源：http://nkr.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://qba.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lfn.hcnkem.com

[R54] 比较两个文件
来源：http://ykx.zdqjudy.top

diff a.txt b.txt
来源：http://ali.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://ggf.cheryme.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bld.cqqwz.cn

[R56] 远程拷贝
来源：http://hpn.xuanzx.com

scp file user@host:/path/
来源：http://tpn.gogol.net.cn

[R57] 远程执行命令
来源：http://qkd.xylfe.cn

ssh user@host 'uptime'
来源：http://aho.chenjidiqi.icu

[R58] 下载文件
来源：http://oeu.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dbg.tianlin.xyz

[R59] 发 POST JSON
来源：http://bit.hnxiangtu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wxm.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://xxd.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vzo.yangfankeji.com

[R61] 磁盘占用
来源：http://ffp.ydzc1.top

df -h;  du -sh *
来源：http://jbo.dashuyun.cn

[R62] 找最占空间的文件
来源：http://dig.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://wmw.svipenyu.cn

[R63] 内存与进程
来源：http://tde.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://mbd.yvedp.cn

[R64] 结束进程
来源：http://nqh.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://odm.kuanghao11.cn

[R65] 查看端口占用
来源：http://kys.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xiw.haohaochexian.top

[R66] 定时任务
来源：http://reu.vqdsnc.cn

crontab -e;  crontab -l
来源：http://mvy.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://rdz.zhoulong.xyz

openssl rand -hex 16
来源：http://azn.iojbl.cn

[R68] 计算文件校验值
来源：http://mmg.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qux.fengsongda.top

[R69] 生成随机密码
来源：http://zmf.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://kot.nanxinkj.top

[R70] 时间戳与互转
来源：http://ihk.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://vjq.yuanzhike.top

[R71] 日期格式化
来源：http://hng.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://sbi.guowangkeji.top

[R72] 等待端口就绪
来源：http://ote.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fnc.shuidangran.top

[R73] 分割大日志
来源：http://xgq.hywenlv.cn

split -l 1000 big.log part_
来源：http://gua.yongpay.top

[R74] 批量重命名
来源：http://fyh.jqgfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://naf.yueranfly.top

[R75] 导出环境变量
来源：http://zgy.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://txx.hywenlv.cn

[R76] 使用临时文件
来源：http://nsp.dianchejie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mib.daxiang520.top

[R77] 读取用户输入
来源：http://olb.vehdjk.com

read -rp "请输入: " ans
来源：http://goc.zhiwuduotai.top

[R78] 交互式菜单
来源：http://hus.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kyo.guannengcc.top

[R79] 解析命令行选项
来源：http://uel.ivvv.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wfi.uphjek.com

[R80] 查看脚本执行耗时
来源：http://mvh.jqgufenzy.top

time ./run.sh
来源：http://dkj.yonumen.top

================================================================================
来源：http://wzt.yanxiufei.cn

S. C / C++ 专题
来源：http://yqd.meibo888.top

================================================================================
来源：http://tco.bjfxy.top

[S01] C：Hello World
来源：http://qdh.dashuyun.cn

#include <stdio.h>
来源：http://uwd.316326.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://umm.hnqzz.top

[S02] C：变量与格式化输出
来源：http://umu.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://kyv.feifeiyinyue.top

[S03] C：读入整数
来源：http://uoy.ybcxt.top

int x; scanf("%d", &x);
来源：http://paw.wangshuangyany.cn

[S04] C：字符串复制
来源：http://vll.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://fyn.daria6918.cn

[S05] C：字符串长度
来源：http://jzq.yj20258888.top

strlen(s)
来源：http://ppx.sufxvd.cn

[S06] C：字符串比较
来源：http://vur.xinyue.icu

strcmp(a, b) == 0
来源：http://cxb.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://lwz.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ymb.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://kxc.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kvp.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://znu.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ozq.iojbl.cn

[S10] C：指针与解引用
来源：http://fmo.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://mhv.yj20258888.top

[S11] C：逐行读文件
来源：http://sxp.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://yqj.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eth.jqgufenzy.top

fclose(f);
来源：http://ips.hfpthk.cn

[S12] C：写文件
来源：http://bry.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zdt.gaohongyu789.top

[S13] C：宏定义
来源：http://nwk.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jsg.sweek.top

[S14] C：枚举
来源：http://blb.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://nen.aibaodan.cn

[S15] C：类型转换
来源：http://xrh.sxryk.cn

(double) a / b
来源：http://oxp.aibaodan.cn

[S16] C：位操作置位
来源：http://jfs.tianlin.xyz

x |= (1 << 3);
来源：http://tbn.xylfe.cn

[S17] C：安全拼接字符串
来源：http://gez.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ojl.fehbvm.com

[S18] C：命令行参数
来源：http://teb.dashuyun.cn

int main(int argc, char **argv)
来源：http://xju.jianghu66.top

[S19] C：快速排序
来源：http://pwm.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aqc.cdnleiting.top

[S20] C：二分查找
来源：http://uxm.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eyn.jiagoushi.top

[S21] C：字符类别判断
来源：http://tup.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gwk.sysykeji.top

[S22] C：字符串转数字
来源：http://jam.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://dhz.0kj1m.cn

[S23] C：随机数
来源：http://wyi.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://upq.yj20258.top

[S24] C：获取本地时间
来源：http://qqv.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ehi.jianghu66.top

[S25] C：内存拷贝
来源：http://eks.cdnleiting.top

memcpy(dst, src, n);
来源：http://ukz.zdbjq.cn

[S26] C：内存清零
来源：http://dpj.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://vpx.yj20258888.top

[S27] C：定义常量
来源：http://occ.yj20258.top

const double PI = 3.14159;
来源：http://bky.sysykeji.top

[S28] C：静态变量
来源：http://cmk.yangfankeji.com

static int counter = 0;
来源：http://kwq.shzxlz.cn

[S29] C：变参函数
来源：http://vlj.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lhd.mhx1999.top

[S30] C：头文件保护
来源：http://cqq.zhijiandao.cn

#ifndef X_H
来源：http://xue.nwbrower.top

#define X_H
来源：http://few.jinqigfzy.top

#endif
来源：http://pua.hysaishi.cn

[S31] C++：Hello World
来源：http://bxf.zhoulong.xyz

#include <iostream>
来源：http://vxi.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://ssq.fengsongda.top

[S32] C++：字符串
来源：http://yok.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://vkc.xziqi.cn

[S33] C++：vector 增删
来源：http://jkk.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sud.nanxinkj.top

[S34] C++：遍历 vector
来源：http://sho.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://nfm.ivvv.top


<!-- 参考信息 -->