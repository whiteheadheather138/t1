代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lgf.zhixingplan.top

[Q26] 计数
来源：http://uzy.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://dcd.xuetiantiany.cn

[Q27] 条件计数
来源：http://dds.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kxj.jinqigfzy.top

[Q28] 求和与平均
来源：http://vrd.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dmu.dianchejie.cn

[Q29] 最大最小值
来源：http://tpd.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://inm.hfpthk.cn

[Q30] 分组统计
来源：http://rxq.tarul.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ame.cdnleiting.top

[Q31] 分组后过滤
来源：http://jol.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vtl.zhixingplan.top

[Q32] 分组拼接字符串
来源：http://sjs.kuanghao11.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://odt.ctjpmb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rlg.feifeiyinyue.top

[Q33] 多列分组
来源：http://ogt.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://efc.yuxming.cn

[Q34] 每组取第一条
来源：http://lfr.jqgufenzy.top

SELECT * FROM (
来源：http://qvp.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sid.haohaochexian.top

) t WHERE rn = 1;
来源：http://ywz.shzxlz.cn

[Q35] 内连接
来源：http://yzc.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gxs.hysaishi.cn

[Q36] 左连接
来源：http://aca.jiagoushi.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pbc.cucudq.cn

[Q37] 右连接
来源：http://hqo.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jbn.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://qsk.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wej.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://enr.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ycd.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://slt.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cdy.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://scy.dianchejie.cn

[Q41] 多表连接
来源：http://puf.cucudq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zlr.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://ayl.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://vze.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://coq.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://aqk.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fxa.hysaishi.cn

[Q43] 标量子查询
来源：http://wje.uphjek.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jrg.guannengcc.top

[Q44] IN 子查询
来源：http://udw.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qvi.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://mjz.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://spd.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://dhl.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oyi.daria6918.cn

[Q47] 与平均值比较
来源：http://gix.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://niu.fengsongda.top

[Q48] CTE 公用表表达式
来源：http://piz.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wlo.guowangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://thx.yonumen.top

[Q49] 更新单行
来源：http://tvu.hfpthk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zev.sweek.top

[Q50] 批量更新
来源：http://eoa.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xse.yuanzhike.top

[Q51] 用子查询更新
来源：http://jfu.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xnx.tarul.cn

[Q52] 删除指定行
来源：http://zmp.vehdjk.com

DELETE FROM users WHERE id = 10;
来源：http://cjt.aizwys.cn

[Q53] 按条件删除
来源：http://lxg.zhijiandao.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nrn.chenjidiqi.icu

[Q54] 清空表
来源：http://fwe.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://izk.nwbrower.top

[Q55] 排名（并列占位）
来源：http://fax.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hri.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://szp.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sbb.havefunace.top

[Q57] 行号
来源：http://bln.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wqs.bbcook.cn

[Q58] 累计求和
来源：http://yhc.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ddb.kuanghao11.cn

[Q59] 分组内累计
来源：http://iqm.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ujm.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://rfg.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hpk.xinyue.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xqd.xuetiantiany.cn

[Q61] 移动平均
来源：http://khr.yuanzhike.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zik.mhx1999.top

[Q62] 分组占比
来源：http://xjw.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kpn.daria6918.cn

[Q63] 开启事务
来源：http://aee.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tgu.mhx1999.top

[Q64] 提交事务
来源：http://knc.guannengcc.top

COMMIT;
来源：http://frv.bbcook.cn

[Q65] 回滚事务
来源：http://woo.svipenyu.cn

ROLLBACK;
来源：http://sns.guannengcc.top

[Q66] 行锁查询
来源：http://rqk.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://knm.jqgfzy.top

[Q67] 设置隔离级别
来源：http://ucv.fehbvm.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ewj.hnxiangtu.top

[Q68] 保存点
来源：http://mjk.vqdsnc.cn

SAVEPOINT sp1;
来源：http://fjm.yfazqb.com

ROLLBACK TO sp1;
来源：http://gls.gotoacloud.top

[Q69] 查看执行计划
来源：http://fie.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vqo.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://xxc.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://uwx.tanke756.top

[Q71] 查看建表语句
来源：http://mtb.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dtv.ctjpmb.com

[Q72] 查看索引
来源：http://ppb.mhx1999.top

SHOW INDEX FROM users;
来源：http://gjx.gogol.net.cn

[Q73] 查看表状态
来源：http://ook.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lag.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://kpe.sweek.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xuv.uphjek.com

[Q75] 日期格式化
来源：http://joy.smart0.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ysu.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ltr.gotoacloud.top

[Q76] 按天统计
来源：http://xjy.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fmz.fengsongda.top

[Q77] 时间加减
来源：http://hzc.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bul.ydzc1.top

[Q78] 当前时间
来源：http://gpt.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hlc.pycfn.com

[Q79] 字符串拼接
来源：http://lwf.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qow.smart0.xyz

[Q80] 字符串截取
来源：http://ses.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zpq.sysykeji.top

[Q81] 字符串替换
来源：http://qki.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://djd.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://beq.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qwa.kuanghao11.cn

[Q83] 大小写转换
来源：http://fsz.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://svb.xylfe.cn

[Q84] 去除首尾空格
来源：http://ctx.yfazqb.com

SELECT TRIM(name) FROM users;
来源：http://lht.zdbjq.cn

[Q85] 数值取整
来源：http://bsp.bbcook.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fph.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://bfm.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hwr.sweek.top

[Q87] JSON 字段做条件
来源：http://nlu.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gfr.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://elu.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kyf.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://imh.redwolf501.top

[Q89] 判断表是否存在
来源：http://yve.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zfp.zdbjq.cn

[Q90] 生成序号列
来源：http://toa.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zfp.quarkkingdee.top

================================================================================
来源：http://gli.birdmap.top

R. Bash 专题
来源：http://gmj.zdqjudy.top

================================================================================
来源：http://vul.vehdjk.com

[R01] shebang 与严格模式
来源：http://rqb.uphjek.com

#!/usr/bin/env bash
来源：http://bfy.yongpay.top

set -euo pipefail
来源：http://jma.svipenyu.cn

[R02] 变量赋值与使用
来源：http://vsh.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://rue.fengsongda.top

[R03] 只读变量
来源：http://hcf.smart0.xyz

readonly PI=3.14
来源：http://oqw.shzxlz.cn

[R04] 位置参数
来源：http://niy.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pxp.fktsv.cn

[R05] 参数默认值
来源：http://glp.cqqwz.cn

name="${1:-default}"
来源：http://evy.sweek.top

[R06] 判断命令是否存在
来源：http://wqg.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jhi.yongpay.top

[R07] if 判断文件
来源：http://nsg.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ahc.aizwys.cn

[R08] 数值比较
来源：http://lxf.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://shv.zycfv.cn

[R09] 字符串比较
来源：http://rnm.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xqq.sxryk.cn

[R10] 正则匹配
来源：http://nmn.yuanzhike.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rww.shanyushiyangtech.top

[R11] case 多分支
来源：http://hay.birdmap.top

case "$1" in
来源：http://vws.ybcxt.top

start) echo "启动" ;;
来源：http://gff.jlsjyb.cn

stop)  echo "停止" ;;
来源：http://zdj.hongshengwenyu.top

*)     echo "未知命令" ;;
来源：http://grf.hesvh.cn

esac
来源：http://bjy.yongpay.top

[R12] for 遍历文件
来源：http://vlz.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://vuv.sweek.top

[R13] for 计数循环
来源：http://pqc.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://ldv.gaohongyu789.top

[R14] C 风格 for
来源：http://yrn.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ytb.shzxlz.cn

[R15] while 逐行读文件
来源：http://tqm.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ucg.redwolf501.top

[R16] until 等待条件
来源：http://ptn.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ohe.ybcxt.top

[R17] 数组定义与取值
来源：http://apj.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://agb.hnqzz.top

[R18] 遍历数组
来源：http://pmh.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dyw.wangdashe.top

[R19] 数组长度
来源：http://xkk.nanxinkj.top

echo "${#arr[@]}"
来源：http://bjh.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://duy.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://drm.hfpthk.cn

[R21] 字符串长度
来源：http://znd.xuanzx.com

echo "${#s}"
来源：http://uyf.aizwys.cn

[R22] 截取子串
来源：http://ktk.havefunace.top

echo "${s:0:5}"
来源：http://xzq.jianghu66.top

[R23] 字符串替换
来源：http://eon.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aek.nwbrower.top

[R24] 大小写转换
来源：http://bbi.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://afk.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://lxh.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cen.cqqwz.cn

[R26] 命令替换
来源：http://cwa.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://bed.aibaodan.cn

[R27] 算术展开
来源：http://eun.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://rsb.daxiang520.top

[R28] 浮点运算
来源：http://lyt.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://ath.jyoumei.cn

[R29] 定义函数
来源：http://fjd.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://adp.fengsongda.top

[R30] 函数返回状态码
来源：http://ppz.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://aft.shuidangran.top

[R31] 局部变量
来源：http://aqo.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://hgz.nanxinkj.top

[R32] 参数个数校验
来源：http://rzv.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://abh.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://pgv.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tvg.tian-w.cn

[R34] 退出时清理
来源：http://scx.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://sgt.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://epu.meibo888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fyv.jyoumei.cn

[R36] 并发执行多个任务
来源：http://tzg.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nfn.bbcook.cn

[R37] 把输出赋给变量
来源：http://dgs.xziqi.cn

files=$(ls -1)
来源：http://wdi.jqgufenzy.top

[R38] 管道串联
来源：http://vri.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://jcp.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://smy.fktsv.cn

cmd > out.log 2>&1
来源：http://ttz.dashuyun.cn

[R40] 追加写日志
来源：http://pqh.tian-w.cn

echo "log" >> out.log
来源：http://pja.ydzc1.top

[R41] 丢弃输出
来源：http://ktz.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://ull.nanxinkj.top

[R42] 输入重定向
来源：http://pzy.shuidangran.top

wc -l < a.txt
来源：http://yit.daria6918.cn

[R43] 按名字查找文件
来源：http://blb.cucudq.cn

find . -name "*.log" -type f
来源：http://alb.xuanzx.com

[R44] 按修改时间查找
来源：http://jwk.chenzaomai.com

find . -mtime -7 -type f
来源：http://ntw.9152youxi.cn

[R45] 批量删除
来源：http://smt.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://hmz.zhengqikj.top

[R46] 递归替换文件内容
来源：http://ktd.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rne.xuetiantiany.cn

[R47] sed 单行替换
来源：http://dhy.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fti.hesvh.cn

[R48] awk 取指定列
来源：http://wlk.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://aev.dashuyun.cn

[R49] awk 带条件
来源：http://xdj.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jkb.ctjpmb.com

[R50] awk 求和
来源：http://lxk.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kda.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://vhh.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lik.yj20258.top

[R52] 统计行数
来源：http://jod.yanxiufei.cn

wc -l a.txt
来源：http://ssc.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://jhv.zdqjudy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ysg.meibo888.top

[R54] 比较两个文件
来源：http://jgv.daria6918.cn

diff a.txt b.txt
来源：http://grq.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://mvk.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rvk.ivvv.top

[R56] 远程拷贝
来源：http://oml.zhiwuduotai.top

scp file user@host:/path/
来源：http://cvm.yfazqb.com

[R57] 远程执行命令
来源：http://dcb.jianghu66.top

ssh user@host 'uptime'
来源：http://rxg.hfpthk.cn

[R58] 下载文件
来源：http://avf.ydzc1.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bwu.dashuyun.cn

[R59] 发 POST JSON
来源：http://uno.chenzaomai.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vzc.ehwqpu.com

[R60] 只看 HTTP 状态码
来源：http://crk.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xra.tarul.cn

[R61] 磁盘占用
来源：http://szn.gzhubu.top

df -h;  du -sh *
来源：http://mvn.sufxvd.cn

[R62] 找最占空间的文件
来源：http://uwc.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://zys.hywenlv.cn

[R63] 内存与进程
来源：http://dhn.fzhhl.top

free -h;  ps aux | grep nginx
来源：http://cns.zhaomingkeji.xyz

[R64] 结束进程
来源：http://njo.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://azk.birdmap.top

[R65] 查看端口占用
来源：http://iji.dashuyun.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bfw.hnxiangtu.top

[R66] 定时任务
来源：http://qth.ehwqpu.com

crontab -e;  crontab -l
来源：http://pho.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://nie.sweek.top

openssl rand -hex 16
来源：http://pkf.fktsv.cn

[R68] 计算文件校验值
来源：http://zuh.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://nvh.nanxinkj.top

[R69] 生成随机密码
来源：http://xiy.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://mhx.jlsjyb.cn

[R70] 时间戳与互转
来源：http://ror.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://qej.redwolf501.top

[R71] 日期格式化
来源：http://nyy.hcnkem.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://yrw.ppjwa.cn

[R72] 等待端口就绪
来源：http://avl.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fhz.birdmap.top

[R73] 分割大日志
来源：http://elp.smart0.xyz

split -l 1000 big.log part_
来源：http://rfn.fehbvm.com

[R74] 批量重命名
来源：http://ckz.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vpn.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://kli.yuxming.cn


<!-- 参考信息 -->