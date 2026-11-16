代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://waj.wangdashe.top

[Q11] 一次插入多行
来源：http://ecx.yuanzhike.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://okk.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://rrw.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://mes.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bwx.fktsv.cn

[Q13] 忽略重复插入
来源：http://ypr.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fck.gogol.net.cn

[Q14] 存在则更新（upsert）
来源：http://iyq.chenjidiqi.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://swc.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tsr.0kj1m.cn

[Q15] 查询全部
来源：http://mge.hcnkem.com

SELECT * FROM users;
来源：http://ugd.zhoulong.xyz

[Q16] 查询指定列
来源：http://rjw.havefunace.top

SELECT id, name FROM users;
来源：http://jpa.yvedp.cn

[Q17] 条件查询
来源：http://lcz.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ycq.guowangkeji.top

[Q18] 模糊匹配
来源：http://gro.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nlc.ydjk.org.cn

[Q19] 范围查询
来源：http://ovt.zycfv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://omh.hnxiangtu.top

[Q20] IN 列表
来源：http://qlg.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hug.xylfe.cn

[Q21] 空值判断
来源：http://vxv.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://yyd.tian-w.cn

[Q22] 排序
来源：http://uny.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rak.aizwys.cn

[Q23] 分页
来源：http://ioi.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pwt.guowangkeji.top

[Q24] 去重
来源：http://jen.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://duy.ybcxt.top

[Q25] 只取前 N 条
来源：http://ugc.yuanzhike.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mqx.xuanzx.com

[Q26] 计数
来源：http://iiq.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://uax.shuidangran.top

[Q27] 条件计数
来源：http://huf.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kcd.52xcode.cn

[Q28] 求和与平均
来源：http://tqk.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fqx.yuxming.cn

[Q29] 最大最小值
来源：http://vhl.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uer.kuanghao11.cn

[Q30] 分组统计
来源：http://qbi.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dsf.yj202588.top

[Q31] 分组后过滤
来源：http://sfq.52xcode.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qtd.hammf.cn

[Q32] 分组拼接字符串
来源：http://jvp.zdbjq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ahz.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jqb.cheryme.top

[Q33] 多列分组
来源：http://xap.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xdb.chenzaomai.com

[Q34] 每组取第一条
来源：http://jpx.mhx1999.top

SELECT * FROM (
来源：http://fea.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ycw.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://jsc.tian-w.cn

[Q35] 内连接
来源：http://kip.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nvn.9152youxi.cn

[Q36] 左连接
来源：http://qwp.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://biu.feifeiyinyue.top

[Q37] 右连接
来源：http://ljh.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xdk.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ula.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sjt.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://vro.yongpay.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://iyo.bjfxy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://euy.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mnd.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uae.jinqigufen.top

[Q41] 多表连接
来源：http://fzb.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://quq.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://dpo.aizwys.cn

JOIN products p ON p.id = o.product_id;
来源：http://ayw.tian-w.cn

[Q42] 连接条件附加过滤
来源：http://acj.zhoulong.xyz

SELECT u.name, o.amount FROM users u
来源：http://okm.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://epl.mhx1999.top

[Q43] 标量子查询
来源：http://ghm.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lgj.gaohongyu789.top

[Q44] IN 子查询
来源：http://vkj.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mdc.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://fnw.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vof.yj20258888.top

[Q46] NOT EXISTS 判断不存在
来源：http://quq.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hva.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://wql.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yvp.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://buw.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nim.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://rch.birdmap.top

[Q49] 更新单行
来源：http://zre.zhongyouzk.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://and.nanxuanxn.top

[Q50] 批量更新
来源：http://ajc.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pqv.yfazqb.com

[Q51] 用子查询更新
来源：http://qgm.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://utq.daria6918.cn

[Q52] 删除指定行
来源：http://zda.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://fny.guannengcc.top

[Q53] 按条件删除
来源：http://bss.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kfu.guannengcc.top

[Q54] 清空表
来源：http://xro.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://ncg.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://bfj.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://egq.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://yqd.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fad.daxiang520.top

[Q57] 行号
来源：http://dpf.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://prp.shzxlz.cn

[Q58] 累计求和
来源：http://ngd.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jyv.redwolf501.top

[Q59] 分组内累计
来源：http://mtw.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://imx.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://wcc.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xry.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dun.guannengcc.top

[Q61] 移动平均
来源：http://fuc.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nud.hnxiangtu.top

[Q62] 分组占比
来源：http://ldz.ybcxt.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aro.sysykeji.top

[Q63] 开启事务
来源：http://kaz.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jmz.fehbvm.com

[Q64] 提交事务
来源：http://rij.yonumen.top

COMMIT;
来源：http://efl.sufxvd.cn

[Q65] 回滚事务
来源：http://zha.sxryk.cn

ROLLBACK;
来源：http://pzz.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://jrr.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bfb.yanxiufei.cn

[Q67] 设置隔离级别
来源：http://wpp.snrcjt.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dqv.quarkkingdee.top

[Q68] 保存点
来源：http://cpc.hcnkem.com

SAVEPOINT sp1;
来源：http://que.ppjwa.cn

ROLLBACK TO sp1;
来源：http://ynz.zhoulong.xyz

[Q69] 查看执行计划
来源：http://cuv.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mtd.chenzaomai.com

[Q70] 更新统计信息
来源：http://tfa.cheryme.top

ANALYZE TABLE users;
来源：http://abe.tanke756.top

[Q71] 查看建表语句
来源：http://elv.yvedp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dyj.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://twp.hnqzz.top

SHOW INDEX FROM users;
来源：http://yck.aizwys.cn

[Q73] 查看表状态
来源：http://oqf.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rlm.tian-w.cn

[Q74] 强制使用索引
来源：http://txz.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://soc.ppjwa.cn

[Q75] 日期格式化
来源：http://qqj.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ahs.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://krr.jyoumei.cn

[Q76] 按天统计
来源：http://ths.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lmn.sxryk.cn

[Q77] 时间加减
来源：http://pxa.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zbo.meibo888.top

[Q78] 当前时间
来源：http://keb.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bys.nanxinkj.top

[Q79] 字符串拼接
来源：http://vyy.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ixf.yfazqb.com

[Q80] 字符串截取
来源：http://qdq.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ews.shuidangran.top

[Q81] 字符串替换
来源：http://nqe.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lta.pycfn.com

[Q82] 字符长度与字节长度
来源：http://oja.hfpthk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wez.fengsongda.top

[Q83] 大小写转换
来源：http://xvd.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jkd.zhixingplan.top

[Q84] 去除首尾空格
来源：http://nju.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://gnk.jlsjyb.cn

[Q85] 数值取整
来源：http://mkj.aibaodan.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iny.andypj.xyz

[Q86] 读取 JSON 字段
来源：http://tow.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dba.xinyue.icu

[Q87] JSON 字段做条件
来源：http://rrj.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vjq.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://arb.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jli.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uev.sxryk.cn

[Q89] 判断表是否存在
来源：http://hib.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://koj.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://iri.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://toa.hysaishi.cn

================================================================================
来源：http://nxu.gzhubu.top

R. Bash 专题
来源：http://oif.guowangkeji.top

================================================================================
来源：http://qgl.sxryk.cn

[R01] shebang 与严格模式
来源：http://ety.jianghu66.top

#!/usr/bin/env bash
来源：http://nje.yuxming.cn

set -euo pipefail
来源：http://tef.0kj1m.cn

[R02] 变量赋值与使用
来源：http://udv.yonumen.top

name="Tom"; echo "$name"
来源：http://zbq.gaohongyu789.top

[R03] 只读变量
来源：http://gcf.jinghuilouyu.cn

readonly PI=3.14
来源：http://xif.fzhhl.top

[R04] 位置参数
来源：http://iyv.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kgb.hfpthk.cn

[R05] 参数默认值
来源：http://lcj.nwbrower.top

name="${1:-default}"
来源：http://ysj.chenzaomai.com

[R06] 判断命令是否存在
来源：http://qub.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wkh.xziqi.cn

[R07] if 判断文件
来源：http://vko.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nnk.nwbrower.top

[R08] 数值比较
来源：http://nex.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://jok.fehbvm.com

[R09] 字符串比较
来源：http://wcu.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ciy.xuetiantiany.cn

[R10] 正则匹配
来源：http://xnw.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tlq.ydzc1.top

[R11] case 多分支
来源：http://rvv.cqqwz.cn

case "$1" in
来源：http://ukg.ehwqpu.com

start) echo "启动" ;;
来源：http://ood.sufxvd.cn

stop)  echo "停止" ;;
来源：http://grk.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://gne.jyoumei.cn

esac
来源：http://vbx.nanxinkj.top

[R12] for 遍历文件
来源：http://eyw.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://sdc.cucudq.cn

[R13] for 计数循环
来源：http://dha.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://qwa.yangfankeji.com

[R14] C 风格 for
来源：http://rxf.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bfj.hcnkem.com

[R15] while 逐行读文件
来源：http://slg.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ywu.yueranfly.top

[R16] until 等待条件
来源：http://nqh.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fst.ybcxt.top

[R17] 数组定义与取值
来源：http://drl.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://snv.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://amk.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bvr.wangdashe.top

[R19] 数组长度
来源：http://dqq.jlsjyb.cn

echo "${#arr[@]}"
来源：http://apf.hcnkem.com

[R20] 关联数组（字典）
来源：http://kfd.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aay.zhongyouzk.top

[R21] 字符串长度
来源：http://kfn.jinqigufen.top

echo "${#s}"
来源：http://tgn.yangfankeji.com

[R22] 截取子串
来源：http://pco.mhx1999.top

echo "${s:0:5}"
来源：http://geg.aizwys.cn

[R23] 字符串替换
来源：http://qip.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ryz.nanxuanxn.top

[R24] 大小写转换
来源：http://sqm.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://oit.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://gfj.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://aux.yuanzhike.top

[R26] 命令替换
来源：http://edn.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://hrm.ydjk.org.cn

[R27] 算术展开
来源：http://oeu.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://ece.feifeiyinyue.top

[R28] 浮点运算
来源：http://gbp.vehdjk.com

echo "scale=2; 10/3" | bc
来源：http://dwd.hesvh.cn

[R29] 定义函数
来源：http://teh.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rmw.dashuyun.cn

[R30] 函数返回状态码
来源：http://mma.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://xfn.52xcode.cn

[R31] 局部变量
来源：http://llc.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://dhg.yuxming.cn

[R32] 参数个数校验
来源：http://fpc.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://arw.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://wmu.hfpthk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ywk.316326.xyz

[R34] 退出时清理
来源：http://wgc.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zsd.yonumen.top

[R35] 后台执行并等待
来源：http://kxa.wangdashe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ugw.zhengqikj.top

[R36] 并发执行多个任务
来源：http://mak.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ywl.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://lww.0kj1m.cn

files=$(ls -1)
来源：http://ica.tarul.cn

[R38] 管道串联
来源：http://vee.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://dfo.jinqigfzy.top

[R39] 重定向标准输出与错误
来源：http://zhu.c1oappe.top

cmd > out.log 2>&1
来源：http://juz.fehbvm.com

[R40] 追加写日志
来源：http://gdb.jyoumei.cn

echo "log" >> out.log
来源：http://dif.shangyingyoupin.top

[R41] 丢弃输出
来源：http://gpd.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://oyu.epnwcf.com

[R42] 输入重定向
来源：http://ubt.jinghuilouyu.cn

wc -l < a.txt
来源：http://elp.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://ikp.gzhubu.top

find . -name "*.log" -type f
来源：http://doi.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://gvd.daxiang520.top

find . -mtime -7 -type f
来源：http://mkh.zhengqikj.top

[R45] 批量删除
来源：http://fpl.guannengcc.top

find . -name "*.tmp" -delete
来源：http://dka.bjfxy.top

[R46] 递归替换文件内容
来源：http://xzi.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mzz.feifeiyinyue.top

[R47] sed 单行替换
来源：http://xmq.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ufd.zhiwuduotai.top

[R48] awk 取指定列
来源：http://jzd.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://plb.daxiang520.top

[R49] awk 带条件
来源：http://jse.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fav.yj20258888.top

[R50] awk 求和
来源：http://rxb.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://kyw.xziqi.cn

[R51] 排序去重取前几
来源：http://zbd.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kut.smart0.xyz

[R52] 统计行数
来源：http://utp.hnxiangtu.top

wc -l a.txt
来源：http://lmr.sysykeji.top

[R53] 查看文件头与实时尾
来源：http://tzm.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zgl.ydzc1.top

[R54] 比较两个文件
来源：http://rtv.yanxiufei.cn

diff a.txt b.txt
来源：http://jfo.jinqigfzy.top

[R55] 压缩与解压
来源：http://fep.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bqp.hnxiangtu.top

[R56] 远程拷贝
来源：http://eou.cucudq.cn

scp file user@host:/path/
来源：http://wqw.mhx1999.top

[R57] 远程执行命令
来源：http://hoj.zdbjq.cn

ssh user@host 'uptime'
来源：http://muj.bjfxy.top

[R58] 下载文件
来源：http://ezn.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tte.hysaishi.cn

[R59] 发 POST JSON
来源：http://mev.guowangkeji.top


<!-- 参考信息 -->