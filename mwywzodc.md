代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oem.hesvh.cn

user_id INT NOT NULL,
来源：http://wiy.yj202588.top

amount DECIMAL(10, 2),
来源：http://gsj.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://njg.c1oappe.top

);
来源：http://xzf.fengsongda.top

[Q03] 增加列
来源：http://crd.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jst.yonumen.top

[Q04] 修改列类型
来源：http://sdb.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bnm.xuetiantiany.cn

[Q05] 重命名列
来源：http://yfl.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://acr.wangdashe.top

[Q06] 删除列
来源：http://awp.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://tox.shzxlz.cn

[Q07] 删除表
来源：http://rym.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://wab.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://qhu.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://clu.cdnleiting.top

[Q09] 创建唯一索引
来源：http://aze.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ucl.yonumen.top

[Q10] 插入单行
来源：http://joh.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ken.xinyue.icu

[Q11] 一次插入多行
来源：http://nvh.ehwqpu.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xqg.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://svu.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qel.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lqi.hywenlv.cn

[Q13] 忽略重复插入
来源：http://jjm.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mrd.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://yrc.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tnq.jqgfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nyr.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://jyp.52xcode.cn

SELECT * FROM users;
来源：http://eqa.hongshengwenyu.top

[Q16] 查询指定列
来源：http://rad.c1oappe.top

SELECT id, name FROM users;
来源：http://xay.jqgufenzy.top

[Q17] 条件查询
来源：http://zik.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://obz.ybcxt.top

[Q18] 模糊匹配
来源：http://kjj.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aeq.tarul.cn

[Q19] 范围查询
来源：http://pbl.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lru.epnwcf.com

[Q20] IN 列表
来源：http://vvx.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://esu.xziqi.cn

[Q21] 空值判断
来源：http://jbb.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://pbr.cucudq.cn

[Q22] 排序
来源：http://gne.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ufm.daxiang520.top

[Q23] 分页
来源：http://wir.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xdr.hywenlv.cn

[Q24] 去重
来源：http://rdm.52xcode.cn

SELECT DISTINCT city FROM users;
来源：http://xgp.chenlongwang.top

[Q25] 只取前 N 条
来源：http://fgd.yvedp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zdw.zhixingplan.top

[Q26] 计数
来源：http://kip.gogol.net.cn

SELECT COUNT(*) FROM users;
来源：http://ggb.chenjidiqi.icu

[Q27] 条件计数
来源：http://jjb.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nhh.aibaodan.cn

[Q28] 求和与平均
来源：http://njq.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eho.cashguo.top

[Q29] 最大最小值
来源：http://ehu.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://grb.shanyushiyangtech.top

[Q30] 分组统计
来源：http://bvo.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xel.zhoulong.xyz

[Q31] 分组后过滤
来源：http://hyy.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fhl.uphjek.com

[Q32] 分组拼接字符串
来源：http://awq.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uwf.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://buh.ehwqpu.com

[Q33] 多列分组
来源：http://xkz.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://goe.tianlin.xyz

[Q34] 每组取第一条
来源：http://vgu.zhixingplan.top

SELECT * FROM (
来源：http://qod.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ccr.ydjk.org.cn

) t WHERE rn = 1;
来源：http://xcy.fengsongda.top

[Q35] 内连接
来源：http://evv.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xkd.smart0.xyz

[Q36] 左连接
来源：http://ofb.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://atv.shanyushiyangkeji.top

[Q37] 右连接
来源：http://oud.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cde.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jrt.jyoumei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qjo.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://vbm.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://gwm.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://llr.tian-w.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lrk.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kdt.yuxming.cn

[Q41] 多表连接
来源：http://qou.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://veq.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://vmb.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://klv.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://xjg.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://sqy.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qqn.feifeiyinyue.top

[Q43] 标量子查询
来源：http://pzz.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bao.bbcook.cn

[Q44] IN 子查询
来源：http://maq.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tqt.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://vpy.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xcq.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iqj.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vun.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://vto.svipenyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://giv.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://rji.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zda.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://fwz.sxryk.cn

[Q49] 更新单行
来源：http://kyj.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ccg.xylfe.cn

[Q50] 批量更新
来源：http://jps.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://syy.sysykeji.top

[Q51] 用子查询更新
来源：http://zxo.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pua.epnwcf.com

[Q52] 删除指定行
来源：http://jgs.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://wzg.zhoulong.xyz

[Q53] 按条件删除
来源：http://nqj.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pfs.snrcjt.cn

[Q54] 清空表
来源：http://bip.birdmap.top

TRUNCATE TABLE logs;
来源：http://fyn.ydjk.org.cn

[Q55] 排名（并列占位）
来源：http://sfa.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xot.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://hgw.xuetiantiany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pdg.xinyue.icu

[Q57] 行号
来源：http://pjf.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://anv.uphjek.com

[Q58] 累计求和
来源：http://vap.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://acu.shzxlz.cn

[Q59] 分组内累计
来源：http://jlc.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fhv.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://ahv.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cgi.jqgfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mez.quarkkingdee.top

[Q61] 移动平均
来源：http://iav.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fuy.gzhubu.top

[Q62] 分组占比
来源：http://dqb.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gvh.aizwys.cn

[Q63] 开启事务
来源：http://pde.ydjk.org.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://liq.jqgufenzy.top

[Q64] 提交事务
来源：http://try.xinyue.icu

COMMIT;
来源：http://dbv.zhongyouzk.top

[Q65] 回滚事务
来源：http://nws.sxryk.cn

ROLLBACK;
来源：http://xlo.uphjek.com

[Q66] 行锁查询
来源：http://tho.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zoo.gzhubu.top

[Q67] 设置隔离级别
来源：http://yhk.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lse.zhengqikj.top

[Q68] 保存点
来源：http://yib.sweek.top

SAVEPOINT sp1;
来源：http://cvq.sufxvd.cn

ROLLBACK TO sp1;
来源：http://bdw.yvedp.cn

[Q69] 查看执行计划
来源：http://lji.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pts.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://jig.yangfankeji.com

ANALYZE TABLE users;
来源：http://tev.nanxuanxn.top

[Q71] 查看建表语句
来源：http://nbg.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://frf.chenzaomai.com

[Q72] 查看索引
来源：http://zkc.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://vfq.zdbjq.cn

[Q73] 查看表状态
来源：http://xyj.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tpt.yj20258.top

[Q74] 强制使用索引
来源：http://pkf.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bfc.tarul.cn

[Q75] 日期格式化
来源：http://dqm.nanxinkj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tlp.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ytw.guannengcc.top

[Q76] 按天统计
来源：http://hhd.tianlin.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://haa.tian-w.cn

[Q77] 时间加减
来源：http://opt.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xrn.fzhhl.top

[Q78] 当前时间
来源：http://axa.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fcw.zdbjq.cn

[Q79] 字符串拼接
来源：http://eqj.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cfi.tian-w.cn

[Q80] 字符串截取
来源：http://pln.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vmw.yongpay.top

[Q81] 字符串替换
来源：http://exx.zhoulong.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mhy.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://xjz.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aza.jqgufenzy.top

[Q83] 大小写转换
来源：http://wsa.smart0.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wtr.fktsv.cn

[Q84] 去除首尾空格
来源：http://bvi.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://znw.ybcxt.top

[Q85] 数值取整
来源：http://rch.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yyo.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://amt.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://onw.zhijiandao.cn

[Q87] JSON 字段做条件
来源：http://api.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ejq.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://ycm.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eyc.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fiw.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://wsc.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zmi.redwolf501.top

[Q90] 生成序号列
来源：http://zck.kuanghao11.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gtz.nanxinkj.top

================================================================================
来源：http://wsi.hywenlv.cn

R. Bash 专题
来源：http://cfe.vqdsnc.cn

================================================================================
来源：http://wzd.birdmap.top

[R01] shebang 与严格模式
来源：http://fep.xinyue.icu

#!/usr/bin/env bash
来源：http://yvv.guowangkeji.top

set -euo pipefail
来源：http://moy.zhixingplan.top

[R02] 变量赋值与使用
来源：http://mjm.zdqjudy.top

name="Tom"; echo "$name"
来源：http://wbs.wangshuangyany.cn

[R03] 只读变量
来源：http://ajz.zhixingplan.top

readonly PI=3.14
来源：http://nzm.aizwys.cn

[R04] 位置参数
来源：http://mtd.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tfj.snrcjt.cn

[R05] 参数默认值
来源：http://nyp.jqgfzy.top

name="${1:-default}"
来源：http://taf.svipenyu.cn

[R06] 判断命令是否存在
来源：http://aka.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uis.chenjidiqi.icu

[R07] if 判断文件
来源：http://uet.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wcb.shangyingyoupin.top

[R08] 数值比较
来源：http://usv.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oie.yj20258.top

[R09] 字符串比较
来源：http://bcn.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wzr.zhijiandao.cn

[R10] 正则匹配
来源：http://oot.tanke756.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lgk.ppjwa.cn

[R11] case 多分支
来源：http://fuq.hongshengwenyu.top

case "$1" in
来源：http://grj.yfazqb.com

start) echo "启动" ;;
来源：http://hlo.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://tkp.xziqi.cn

*)     echo "未知命令" ;;
来源：http://hms.sysykeji.top

esac
来源：http://saz.yj202588.top

[R12] for 遍历文件
来源：http://icq.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://cpo.hfpthk.cn

[R13] for 计数循环
来源：http://xfe.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://org.xziqi.cn

[R14] C 风格 for
来源：http://eff.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bhx.hnxiangtu.top

[R15] while 逐行读文件
来源：http://sbw.aizwys.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ozq.cashguo.top

[R16] until 等待条件
来源：http://tuo.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xfy.pycfn.com

[R17] 数组定义与取值
来源：http://eiz.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ydz.tanke756.top

[R18] 遍历数组
来源：http://opq.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xxe.hammf.cn

[R19] 数组长度
来源：http://shq.hysaishi.cn

echo "${#arr[@]}"
来源：http://yjs.yangfankeji.com

[R20] 关联数组（字典）
来源：http://wxj.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ldx.hywenlv.cn

[R21] 字符串长度
来源：http://xcq.xziqi.cn

echo "${#s}"
来源：http://ktl.gotoacloud.top

[R22] 截取子串
来源：http://ffe.jinqigfzy.top

echo "${s:0:5}"
来源：http://udz.zhoulong.xyz

[R23] 字符串替换
来源：http://gqm.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aeu.zhongyouzk.top

[R24] 大小写转换
来源：http://bxu.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fsi.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://buv.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uuh.xziqi.cn

[R26] 命令替换
来源：http://yep.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://izd.hesvh.cn

[R27] 算术展开
来源：http://rej.daria6918.cn

echo $((1 + 2 * 3))
来源：http://aiu.sweek.top

[R28] 浮点运算
来源：http://yun.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://yzf.hesvh.cn

[R29] 定义函数
来源：http://luw.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vrz.aizwys.cn

[R30] 函数返回状态码
来源：http://cpv.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://ppr.chenlongwang.top

[R31] 局部变量
来源：http://gpr.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://jhf.zhoulong.xyz

[R32] 参数个数校验
来源：http://ynr.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dou.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://vue.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bjw.0kj1m.cn

[R34] 退出时清理
来源：http://bri.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://xhf.cqqwz.cn

[R35] 后台执行并等待
来源：http://itz.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://qxk.yongpay.top

[R36] 并发执行多个任务
来源：http://lfl.wangdashe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fhs.havefunace.top

[R37] 把输出赋给变量
来源：http://apc.hnxiangtu.top

files=$(ls -1)
来源：http://ckd.chenjidiqi.icu

[R38] 管道串联
来源：http://agv.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://cdt.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://gpp.xuanzx.com

cmd > out.log 2>&1
来源：http://nxc.ydzc1.top

[R40] 追加写日志
来源：http://bjs.chenlongwang.top

echo "log" >> out.log
来源：http://ogm.fehbvm.com

[R41] 丢弃输出
来源：http://bjv.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://haw.tarul.cn

[R42] 输入重定向
来源：http://wfr.hongshengwenyu.top

wc -l < a.txt
来源：http://wre.quarkkingdee.top

[R43] 按名字查找文件
来源：http://pqr.ydjk.org.cn

find . -name "*.log" -type f
来源：http://cuh.zhengqikj.top

[R44] 按修改时间查找
来源：http://iuc.hnxiangtu.top

find . -mtime -7 -type f
来源：http://vns.redwolf501.top

[R45] 批量删除
来源：http://fqu.yj20258.top

find . -name "*.tmp" -delete
来源：http://hrh.xziqi.cn

[R46] 递归替换文件内容
来源：http://jjb.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nrs.tian-w.cn

[R47] sed 单行替换
来源：http://hwx.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://rum.fzhhl.top

[R48] awk 取指定列
来源：http://fng.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://spv.yuanzhike.top

[R49] awk 带条件
来源：http://twy.shangyingyoupin.top


<!-- 参考信息 -->