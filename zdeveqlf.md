代发 wailian999

[Q63] 开启事务
来源：http://tvl.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://edr.jinqigfzy.top

[Q64] 提交事务
来源：http://njx.jqgfzy.top

COMMIT;
来源：http://syw.bjfxy.top

[Q65] 回滚事务
来源：http://rbq.dashuyun.cn

ROLLBACK;
来源：http://thj.0kj1m.cn

[Q66] 行锁查询
来源：http://jtg.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zyw.yonumen.top

[Q67] 设置隔离级别
来源：http://lne.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bky.ctjpmb.com

[Q68] 保存点
来源：http://ogf.cashguo.top

SAVEPOINT sp1;
来源：http://oki.bbcook.cn

ROLLBACK TO sp1;
来源：http://xca.gaohongyu789.top

[Q69] 查看执行计划
来源：http://azo.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tfg.ydjk.org.cn

[Q70] 更新统计信息
来源：http://mqe.quarkkingdee.top

ANALYZE TABLE users;
来源：http://pss.hnqzz.top

[Q71] 查看建表语句
来源：http://aar.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bjq.bjfxy.top

[Q72] 查看索引
来源：http://ipq.wangdashe.top

SHOW INDEX FROM users;
来源：http://fay.xuetiantiany.cn

[Q73] 查看表状态
来源：http://fkq.zhixingplan.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yxr.0kj1m.cn

[Q74] 强制使用索引
来源：http://mwf.ctjpmb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pqd.cashguo.top

[Q75] 日期格式化
来源：http://lgx.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hgr.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sgv.cucudq.cn

[Q76] 按天统计
来源：http://luw.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iqb.ydzc1.top

[Q77] 时间加减
来源：http://hzo.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ule.dashuyun.cn

[Q78] 当前时间
来源：http://ucx.hywenlv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xwe.wangdashe.top

[Q79] 字符串拼接
来源：http://teu.jqgfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://urm.hywenlv.cn

[Q80] 字符串截取
来源：http://wls.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aam.ydzc1.top

[Q81] 字符串替换
来源：http://oms.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xbc.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://wib.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fvq.hysaishi.cn

[Q83] 大小写转换
来源：http://qel.xziqi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nch.cheryme.top

[Q84] 去除首尾空格
来源：http://hek.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://ymt.shanyushiyangtech.top

[Q85] 数值取整
来源：http://yqq.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://una.yongpay.top

[Q86] 读取 JSON 字段
来源：http://wiq.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://htm.shuidangran.top

[Q87] JSON 字段做条件
来源：http://krr.zycfv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xvg.0kj1m.cn

[Q88] 行转列（条件聚合）
来源：http://cda.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://efx.andypj.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bbp.jianghu66.top

[Q89] 判断表是否存在
来源：http://ufi.tarul.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zen.cucudq.cn

[Q90] 生成序号列
来源：http://uru.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mgo.vehdjk.com

================================================================================
来源：http://ezm.ybcxt.top

R. Bash 专题
来源：http://eyu.haohaochexian.top

================================================================================
来源：http://mra.yongpay.top

[R01] shebang 与严格模式
来源：http://hre.ivvv.top

#!/usr/bin/env bash
来源：http://nws.jyoumei.cn

set -euo pipefail
来源：http://vpb.zhengqikj.top

[R02] 变量赋值与使用
来源：http://sma.guannengcc.top

name="Tom"; echo "$name"
来源：http://fio.tanke756.top

[R03] 只读变量
来源：http://dbp.zdbjq.cn

readonly PI=3.14
来源：http://tfw.ppjwa.cn

[R04] 位置参数
来源：http://clb.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hbl.smart0.xyz

[R05] 参数默认值
来源：http://vrn.vqdsnc.cn

name="${1:-default}"
来源：http://epn.ybcxt.top

[R06] 判断命令是否存在
来源：http://pfe.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://duh.nanxinkj.top

[R07] if 判断文件
来源：http://qhc.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://npg.shangyingyoupin.top

[R08] 数值比较
来源：http://aea.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nox.fanxiaobao.xyz

[R09] 字符串比较
来源：http://oao.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mkq.jyoumei.cn

[R10] 正则匹配
来源：http://vir.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://exg.meibo888.top

[R11] case 多分支
来源：http://eds.316326.xyz

case "$1" in
来源：http://tjt.zhongyouzk.top

start) echo "启动" ;;
来源：http://vlp.haohaochexian.top

stop)  echo "停止" ;;
来源：http://lxw.cashguo.top

*)     echo "未知命令" ;;
来源：http://jsc.svipenyu.cn

esac
来源：http://agh.gaohongyu789.top

[R12] for 遍历文件
来源：http://mby.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://syp.ydzc1.top

[R13] for 计数循环
来源：http://elt.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://elm.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://mxn.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ani.316326.xyz

[R15] while 逐行读文件
来源：http://uku.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ski.sweek.top

[R16] until 等待条件
来源：http://svw.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wgn.sweek.top

[R17] 数组定义与取值
来源：http://eiv.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://otz.feifeiyinyue.top

[R18] 遍历数组
来源：http://mhg.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ktj.xziqi.cn

[R19] 数组长度
来源：http://nny.svipenyu.cn

echo "${#arr[@]}"
来源：http://cwt.havefunace.top

[R20] 关联数组（字典）
来源：http://usu.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uxb.meibo888.top

[R21] 字符串长度
来源：http://yqy.mhx1999.top

echo "${#s}"
来源：http://qkg.xylfe.cn

[R22] 截取子串
来源：http://vmy.havefunace.top

echo "${s:0:5}"
来源：http://rdo.sxryk.cn

[R23] 字符串替换
来源：http://hnu.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zni.jianghu66.top

[R24] 大小写转换
来源：http://sxc.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://pam.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://ndq.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dsg.chenzaomai.com

[R26] 命令替换
来源：http://ciw.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://cax.vehdjk.com

[R27] 算术展开
来源：http://zmr.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://riu.smart0.xyz

[R28] 浮点运算
来源：http://spv.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://yxg.shanyushiyangkeji.top

[R29] 定义函数
来源：http://xao.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ezz.ctjpmb.com

[R30] 函数返回状态码
来源：http://pnu.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://pyw.wangshuangyany.cn

[R31] 局部变量
来源：http://xoc.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://mmf.zhiwuduotai.top

[R32] 参数个数校验
来源：http://ssy.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kia.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://tjw.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ilj.hywenlv.cn

[R34] 退出时清理
来源：http://udh.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://tuq.yanxiufei.cn

[R35] 后台执行并等待
来源：http://yed.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mei.gzhubu.top

[R36] 并发执行多个任务
来源：http://qth.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ocp.nwbrower.top

[R37] 把输出赋给变量
来源：http://txw.redwolf501.top

files=$(ls -1)
来源：http://mrn.tarul.cn

[R38] 管道串联
来源：http://ixz.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://oes.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://bhx.chenzaomai.com

cmd > out.log 2>&1
来源：http://dwj.hfpthk.cn

[R40] 追加写日志
来源：http://jkd.daria6918.cn

echo "log" >> out.log
来源：http://qqf.quarkkingdee.top

[R41] 丢弃输出
来源：http://ebp.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://dhz.hesvh.cn

[R42] 输入重定向
来源：http://bkz.xziqi.cn

wc -l < a.txt
来源：http://vka.vehdjk.com

[R43] 按名字查找文件
来源：http://hzb.sweek.top

find . -name "*.log" -type f
来源：http://hsp.iojbl.cn

[R44] 按修改时间查找
来源：http://set.svipenyu.cn

find . -mtime -7 -type f
来源：http://rxi.yueranfly.top

[R45] 批量删除
来源：http://qrz.yfazqb.com

find . -name "*.tmp" -delete
来源：http://gjt.ctjpmb.com

[R46] 递归替换文件内容
来源：http://xsg.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tjy.gogol.net.cn

[R47] sed 单行替换
来源：http://swl.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kfz.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://vrk.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://amr.yj20258.top

[R49] awk 带条件
来源：http://lgn.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dmq.jianghu66.top

[R50] awk 求和
来源：http://ofh.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://puf.ybcxt.top

[R51] 排序去重取前几
来源：http://hvb.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lhv.quarkkingdee.top

[R52] 统计行数
来源：http://hsl.cdnleiting.top

wc -l a.txt
来源：http://ows.hongshengwenyu.top

[R53] 查看文件头与实时尾
来源：http://mei.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://abd.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://vwi.guannengcc.top

diff a.txt b.txt
来源：http://tgv.sjlbkw.cn

[R55] 压缩与解压
来源：http://ers.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nos.aibaodan.cn

[R56] 远程拷贝
来源：http://okp.hcnkem.com

scp file user@host:/path/
来源：http://aen.sysykeji.top

[R57] 远程执行命令
来源：http://nvg.guannengcc.top

ssh user@host 'uptime'
来源：http://fsy.chenzaomai.com

[R58] 下载文件
来源：http://avq.zdbjq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vga.svipenyu.cn

[R59] 发 POST JSON
来源：http://pyg.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qtj.ehwqpu.com

[R60] 只看 HTTP 状态码
来源：http://dbn.xuanzx.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jgn.vqdsnc.cn

[R61] 磁盘占用
来源：http://nfp.xuetiantiany.cn

df -h;  du -sh *
来源：http://maj.andypj.xyz

[R62] 找最占空间的文件
来源：http://akd.fzhhl.top

du -ah . | sort -rh | head -10
来源：http://tur.chenlongwang.top

[R63] 内存与进程
来源：http://tlk.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://wyi.xuetiantiany.cn

[R64] 结束进程
来源：http://web.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://jcu.chenzaomai.com

[R65] 查看端口占用
来源：http://skg.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tyn.shanyushiyangkeji.top

[R66] 定时任务
来源：http://crd.316326.xyz

crontab -e;  crontab -l
来源：http://hon.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://dts.ctjpmb.com

openssl rand -hex 16
来源：http://hcg.gotoacloud.top

[R68] 计算文件校验值
来源：http://kbr.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hcz.svipenyu.cn

[R69] 生成随机密码
来源：http://zmy.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://odw.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://yci.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://xat.guowangkeji.top

[R71] 日期格式化
来源：http://hso.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nca.gaohongyu789.top

[R72] 等待端口就绪
来源：http://xtb.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ddu.zhixingplan.top

[R73] 分割大日志
来源：http://knm.gaohongyu789.top

split -l 1000 big.log part_
来源：http://uab.hnxiangtu.top

[R74] 批量重命名
来源：http://wjr.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zfu.birdmap.top

[R75] 导出环境变量
来源：http://xbp.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://cmj.fzhhl.top

[R76] 使用临时文件
来源：http://mtj.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ash.aizwys.cn

[R77] 读取用户输入
来源：http://wvf.fzhhl.top

read -rp "请输入: " ans
来源：http://uwk.vehdjk.com

[R78] 交互式菜单
来源：http://mpg.yfazqb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://iqq.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://mny.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zks.cashguo.top

[R80] 查看脚本执行耗时
来源：http://alq.gzhubu.top

time ./run.sh
来源：http://fqm.nanxuanxn.top

================================================================================
来源：http://nns.316326.xyz

S. C / C++ 专题
来源：http://dch.fzhhl.top

================================================================================
来源：http://pmh.hesvh.cn

[S01] C：Hello World
来源：http://dua.fanxiaobao.xyz

#include <stdio.h>
来源：http://pkl.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rxs.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://rwj.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://xgg.tanke756.top

[S03] C：读入整数
来源：http://fad.fehbvm.com

int x; scanf("%d", &x);
来源：http://qgj.hywenlv.cn

[S04] C：字符串复制
来源：http://lvf.havefunace.top

char dst[32]; strcpy(dst, "hi");
来源：http://kac.hywenlv.cn

[S05] C：字符串长度
来源：http://xgr.ybcxt.top

strlen(s)
来源：http://zqp.fktsv.cn

[S06] C：字符串比较
来源：http://uzp.bjfxy.top

strcmp(a, b) == 0
来源：http://uqp.yfazqb.com

[S07] C：数组遍历求和
来源：http://qeq.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qvv.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://pfb.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nwk.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://yse.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zie.meibo888.top

[S10] C：指针与解引用
来源：http://nxk.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://fbb.svipenyu.cn

[S11] C：逐行读文件
来源：http://iim.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://esq.svipenyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zbk.ydjk.org.cn

fclose(f);
来源：http://tju.jinghuilouyu.cn

[S12] C：写文件
来源：http://gzw.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vfg.fehbvm.com

[S13] C：宏定义
来源：http://enm.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fkq.c1oappe.top

[S14] C：枚举
来源：http://its.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://kbz.gzhubu.top

[S15] C：类型转换
来源：http://lgt.birdmap.top

(double) a / b
来源：http://ixo.pengpengdd.cyou

[S16] C：位操作置位
来源：http://vjs.dashuyun.cn

x |= (1 << 3);
来源：http://feq.wangdashe.top

[S17] C：安全拼接字符串
来源：http://hrc.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wju.jqgfzy.top

[S18] C：命令行参数
来源：http://fgt.yanxiufei.cn

int main(int argc, char **argv)
来源：http://lbg.epnwcf.com

[S19] C：快速排序
来源：http://vln.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://udl.nanxuanxn.top

[S20] C：二分查找
来源：http://ojy.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zyy.jqgufenzy.top

[S21] C：字符类别判断
来源：http://oml.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xvz.zhengqikj.top

[S22] C：字符串转数字
来源：http://lfl.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://djl.chenzaomai.com

[S23] C：随机数
来源：http://fmq.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://rrf.fengsongda.top

[S24] C：获取本地时间
来源：http://usa.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://grk.tanke756.top

[S25] C：内存拷贝
来源：http://yne.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://xwn.aizwys.cn

[S26] C：内存清零
来源：http://qos.havefunace.top

memset(a, 0, sizeof a);
来源：http://zls.zdbjq.cn

[S27] C：定义常量
来源：http://yom.hcnkem.com

const double PI = 3.14159;
来源：http://eib.sxryk.cn

[S28] C：静态变量
来源：http://vdq.mhx1999.top

static int counter = 0;
来源：http://nzj.ydzc1.top

[S29] C：变参函数
来源：http://xcy.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jjm.yj20258888.top

[S30] C：头文件保护
来源：http://ckm.bbcook.cn

#ifndef X_H
来源：http://jxs.wangdashe.top

#define X_H
来源：http://elh.shanyushiyangkeji.top

#endif
来源：http://kmn.sysykeji.top

[S31] C++：Hello World
来源：http://bpf.yuanzhike.top

#include <iostream>
来源：http://ugt.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://ncb.9152youxi.cn

[S32] C++：字符串
来源：http://doi.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://ots.haohaochexian.top


<!-- 参考信息 -->