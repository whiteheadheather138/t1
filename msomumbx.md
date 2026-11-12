代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://czn.jyoumei.cn

[Q50] 批量更新
来源：http://kuq.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://juc.smart0.xyz

[Q51] 用子查询更新
来源：http://wuy.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://orp.sufxvd.cn

[Q52] 删除指定行
来源：http://nqw.smart0.xyz

DELETE FROM users WHERE id = 10;
来源：http://xbp.cucudq.cn

[Q53] 按条件删除
来源：http://kqj.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nps.cdnleiting.top

[Q54] 清空表
来源：http://pqa.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://gii.shanyushiyangkeji.top

[Q55] 排名（并列占位）
来源：http://giu.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mbh.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://ggc.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kew.xinyue.icu

[Q57] 行号
来源：http://dgf.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://adg.daria6918.cn

[Q58] 累计求和
来源：http://esj.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jmk.yueranfly.top

[Q59] 分组内累计
来源：http://bgj.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yvz.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://osr.ppjwa.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fun.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://feh.0kj1m.cn

[Q61] 移动平均
来源：http://tpx.vqdsnc.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rrs.hammf.cn

[Q62] 分组占比
来源：http://kcs.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://doh.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://mhz.vehdjk.com

START TRANSACTION;                -- 或 BEGIN
来源：http://zvv.ivvv.top

[Q64] 提交事务
来源：http://xwh.havefunace.top

COMMIT;
来源：http://wnn.cheryme.top

[Q65] 回滚事务
来源：http://gqf.bjfxy.top

ROLLBACK;
来源：http://qti.fengsongda.top

[Q66] 行锁查询
来源：http://dop.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://niz.sysykeji.top

[Q67] 设置隔离级别
来源：http://olt.yuanzhike.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cqa.jinghuilouyu.cn

[Q68] 保存点
来源：http://izh.cucudq.cn

SAVEPOINT sp1;
来源：http://svf.zhengqikj.top

ROLLBACK TO sp1;
来源：http://lpe.sweek.top

[Q69] 查看执行计划
来源：http://bun.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ngx.xuanzx.com

[Q70] 更新统计信息
来源：http://hgn.snrcjt.cn

ANALYZE TABLE users;
来源：http://ldo.fktsv.cn

[Q71] 查看建表语句
来源：http://iqf.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fuz.xylfe.cn

[Q72] 查看索引
来源：http://zbi.yuanzhike.top

SHOW INDEX FROM users;
来源：http://epv.iojbl.cn

[Q73] 查看表状态
来源：http://eml.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ouh.yvedp.cn

[Q74] 强制使用索引
来源：http://gfy.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://adp.gzhubu.top

[Q75] 日期格式化
来源：http://yht.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://egt.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bvw.hongshengwenyu.top

[Q76] 按天统计
来源：http://blj.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qzh.jyoumei.cn

[Q77] 时间加减
来源：http://qmv.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hak.xylfe.cn

[Q78] 当前时间
来源：http://lfr.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hnf.vehdjk.com

[Q79] 字符串拼接
来源：http://jhf.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qgf.chenzaomai.com

[Q80] 字符串截取
来源：http://pxe.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sft.fengsongda.top

[Q81] 字符串替换
来源：http://zwo.havefunace.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jzw.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://jio.tian-w.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mig.zycfv.cn

[Q83] 大小写转换
来源：http://wcz.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oof.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://ovl.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://zuf.9152youxi.cn

[Q85] 数值取整
来源：http://hcz.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ryu.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://qjf.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cnh.yonumen.top

[Q87] JSON 字段做条件
来源：http://cep.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pvu.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://dep.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cqq.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zag.zhengqikj.top

[Q89] 判断表是否存在
来源：http://gjc.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cog.wangdashe.top

[Q90] 生成序号列
来源：http://bfi.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bia.daxiang520.top

================================================================================
来源：http://weo.xylfe.cn

R. Bash 专题
来源：http://jzw.redwolf501.top

================================================================================
来源：http://bgk.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://wbf.andypj.xyz

#!/usr/bin/env bash
来源：http://gxm.tanke756.top

set -euo pipefail
来源：http://zoc.daria6918.cn

[R02] 变量赋值与使用
来源：http://iap.guannengcc.top

name="Tom"; echo "$name"
来源：http://jhi.yj20258.top

[R03] 只读变量
来源：http://cll.yuxming.cn

readonly PI=3.14
来源：http://sex.yongpay.top

[R04] 位置参数
来源：http://ykk.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wmf.ybcxt.top

[R05] 参数默认值
来源：http://lre.guannengcc.top

name="${1:-default}"
来源：http://dqf.cdnleiting.top

[R06] 判断命令是否存在
来源：http://sgq.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cux.cqqwz.cn

[R07] if 判断文件
来源：http://ziy.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hho.hammf.cn

[R08] 数值比较
来源：http://qcu.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://etg.jinqigufen.top

[R09] 字符串比较
来源：http://vgt.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pcn.tian-w.cn

[R10] 正则匹配
来源：http://uco.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ujq.aizwys.cn

[R11] case 多分支
来源：http://npy.yvedp.cn

case "$1" in
来源：http://nfb.gzhubu.top

start) echo "启动" ;;
来源：http://lel.xinyue.icu

stop)  echo "停止" ;;
来源：http://kme.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://ajd.gotoacloud.top

esac
来源：http://evu.shzxlz.cn

[R12] for 遍历文件
来源：http://abx.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://eru.hysaishi.cn

[R13] for 计数循环
来源：http://jfr.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://byh.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://peu.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://drg.yanxiufei.cn

[R15] while 逐行读文件
来源：http://pqf.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yzu.nanxuanxn.top

[R16] until 等待条件
来源：http://kql.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dal.yangfankeji.com

[R17] 数组定义与取值
来源：http://sqo.bbcook.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ksb.redwolf501.top

[R18] 遍历数组
来源：http://qir.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://awj.ydjk.org.cn

[R19] 数组长度
来源：http://lgx.c1oappe.top

echo "${#arr[@]}"
来源：http://dsu.zhengqikj.top

[R20] 关联数组（字典）
来源：http://ubd.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nqn.gogol.net.cn

[R21] 字符串长度
来源：http://qcc.zhoulong.xyz

echo "${#s}"
来源：http://yzb.daria6918.cn

[R22] 截取子串
来源：http://ami.guowangkeji.top

echo "${s:0:5}"
来源：http://jtk.tianlin.xyz

[R23] 字符串替换
来源：http://ptt.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rsk.fzhhl.top

[R24] 大小写转换
来源：http://gfn.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gqa.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://mlk.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uyi.xuetiantiany.cn

[R26] 命令替换
来源：http://ugh.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://xxa.ivvv.top

[R27] 算术展开
来源：http://qek.tanke756.top

echo $((1 + 2 * 3))
来源：http://wzd.iojbl.cn

[R28] 浮点运算
来源：http://vlw.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://gva.hnxiangtu.top

[R29] 定义函数
来源：http://tzp.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kkf.xziqi.cn

[R30] 函数返回状态码
来源：http://xkp.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://xhh.c1oappe.top

[R31] 局部变量
来源：http://wrs.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://hdy.daria6918.cn

[R32] 参数个数校验
来源：http://zev.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gsr.meibo888.top

[R33] 捕获错误并提示行号
来源：http://czg.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qrr.gaohongyu789.top

[R34] 退出时清理
来源：http://wvy.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://gzb.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://mbm.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ahf.guannengcc.top

[R36] 并发执行多个任务
来源：http://cmo.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tls.tanke756.top

[R37] 把输出赋给变量
来源：http://pdo.jinghuilouyu.cn

files=$(ls -1)
来源：http://mga.xuanzx.com

[R38] 管道串联
来源：http://tfx.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://lzu.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://sxb.snrcjt.cn

cmd > out.log 2>&1
来源：http://qyo.jinqigfzy.top

[R40] 追加写日志
来源：http://pel.jlsjyb.cn

echo "log" >> out.log
来源：http://cdm.jqgfzy.top

[R41] 丢弃输出
来源：http://rtt.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://fkc.cashguo.top

[R42] 输入重定向
来源：http://zix.hnqzz.top

wc -l < a.txt
来源：http://jvr.havefunace.top

[R43] 按名字查找文件
来源：http://foz.nanxinkj.top

find . -name "*.log" -type f
来源：http://atp.nanxuanxn.top

[R44] 按修改时间查找
来源：http://ged.chenlongwang.top

find . -mtime -7 -type f
来源：http://sbn.hysaishi.cn

[R45] 批量删除
来源：http://qly.zhaomingkeji.xyz

find . -name "*.tmp" -delete
来源：http://hct.fktsv.cn

[R46] 递归替换文件内容
来源：http://ltx.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nde.yvedp.cn

[R47] sed 单行替换
来源：http://vll.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://azz.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://usg.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://oif.sysykeji.top

[R49] awk 带条件
来源：http://uut.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kta.9152youxi.cn

[R50] awk 求和
来源：http://xej.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://wsi.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://tju.ybcxt.top

sort a.txt | uniq -c | sort -rn | head
来源：http://atm.yuanzhike.top

[R52] 统计行数
来源：http://rvw.jiagoushi.top

wc -l a.txt
来源：http://wfv.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://dil.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gln.9152youxi.cn

[R54] 比较两个文件
来源：http://fwg.haohaochexian.top

diff a.txt b.txt
来源：http://dlj.hongshengwenyu.top

[R55] 压缩与解压
来源：http://rda.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://trh.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://cme.yj20258888.top

scp file user@host:/path/
来源：http://wmb.bjfxy.top

[R57] 远程执行命令
来源：http://liu.meibo888.top

ssh user@host 'uptime'
来源：http://cif.tarul.cn

[R58] 下载文件
来源：http://pmb.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rla.cdnleiting.top

[R59] 发 POST JSON
来源：http://xio.jiagoushi.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tsx.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://ssk.zdbjq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ese.tanke756.top

[R61] 磁盘占用
来源：http://zkt.52xcode.cn

df -h;  du -sh *
来源：http://gtu.hesvh.cn

[R62] 找最占空间的文件
来源：http://udp.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://mff.sufxvd.cn

[R63] 内存与进程
来源：http://dvq.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://uht.nwbrower.top

[R64] 结束进程
来源：http://ddw.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://gcx.jinqigfzy.top

[R65] 查看端口占用
来源：http://ooa.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hwc.daria6918.cn

[R66] 定时任务
来源：http://sin.c1oappe.top

crontab -e;  crontab -l
来源：http://rie.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://pin.yj202588.top

openssl rand -hex 16
来源：http://adx.xylfe.cn

[R68] 计算文件校验值
来源：http://ohn.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://gbb.hywenlv.cn

[R69] 生成随机密码
来源：http://hsg.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://zqt.ivvv.top

[R70] 时间戳与互转
来源：http://dkt.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://kmq.quarkkingdee.top

[R71] 日期格式化
来源：http://qcr.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ijm.nwbrower.top

[R72] 等待端口就绪
来源：http://xpj.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vrz.haohaochexian.top

[R73] 分割大日志
来源：http://zfx.haohaochexian.top

split -l 1000 big.log part_
来源：http://gwz.guowangkeji.top

[R74] 批量重命名
来源：http://cie.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wqs.zhoulong.xyz

[R75] 导出环境变量
来源：http://tnf.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://fnj.cashguo.top

[R76] 使用临时文件
来源：http://yhh.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jxo.fehbvm.com

[R77] 读取用户输入
来源：http://hyh.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://rqy.svipenyu.cn

[R78] 交互式菜单
来源：http://xdm.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nte.svipenyu.cn

[R79] 解析命令行选项
来源：http://mut.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yrn.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://ytt.dashuyun.cn

time ./run.sh
来源：http://tos.jianghu66.top

================================================================================
来源：http://gyj.sysykeji.top

S. C / C++ 专题
来源：http://vjc.guowangkeji.top

================================================================================
来源：http://nat.chenzaomai.com

[S01] C：Hello World
来源：http://nwt.hnqzz.top

#include <stdio.h>
来源：http://ene.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://djn.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://fhu.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://ztj.zhixingplan.top

[S03] C：读入整数
来源：http://rec.hfpthk.cn

int x; scanf("%d", &x);
来源：http://tgb.sxryk.cn

[S04] C：字符串复制
来源：http://pwa.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://eur.yangfankeji.com

[S05] C：字符串长度
来源：http://dmu.jinqigufen.top

strlen(s)
来源：http://nfx.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://gsj.sufxvd.cn

strcmp(a, b) == 0
来源：http://rup.xziqi.cn

[S07] C：数组遍历求和
来源：http://cwy.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://krn.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://clp.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kcj.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://jdv.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dqu.daxiang520.top

[S10] C：指针与解引用
来源：http://aws.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://fyc.dashuyun.cn

[S11] C：逐行读文件
来源：http://hdv.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://cxg.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ruy.zhijiandao.cn

fclose(f);
来源：http://ymh.shuidangran.top

[S12] C：写文件
来源：http://xth.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jzv.daria6918.cn

[S13] C：宏定义
来源：http://roe.wangshuangyany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fmc.hcnkem.com

[S14] C：枚举
来源：http://bcz.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://spy.jqgufenzy.top

[S15] C：类型转换
来源：http://deo.andypj.xyz

(double) a / b
来源：http://txo.hammf.cn

[S16] C：位操作置位
来源：http://tip.cdnleiting.top

x |= (1 << 3);
来源：http://idh.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://kxb.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jbx.sjlbkw.cn

[S18] C：命令行参数
来源：http://zhr.tanke756.top

int main(int argc, char **argv)
来源：http://rsu.sxryk.cn

[S19] C：快速排序
来源：http://bky.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://jjx.hnxiangtu.top

[S20] C：二分查找
来源：http://uiw.gzhubu.top


<!-- 参考信息 -->