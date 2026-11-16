代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ygm.cucudq.cn

);
来源：http://zwq.svipenyu.cn

[Q02] 创建带外键的表
来源：http://luf.zhiwuduotai.top

CREATE TABLE orders (
来源：http://hdm.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tkg.daxiang520.top

user_id INT NOT NULL,
来源：http://trs.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://zdn.gzhubu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mja.hnqzz.top

);
来源：http://uhs.gaohongyu789.top

[Q03] 增加列
来源：http://cmh.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oov.hfpthk.cn

[Q04] 修改列类型
来源：http://ury.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kpu.zhixingplan.top

[Q05] 重命名列
来源：http://weg.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jsd.zhongyouzk.top

[Q06] 删除列
来源：http://vih.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hmo.0kj1m.cn

[Q07] 删除表
来源：http://qvd.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://oeo.yvedp.cn

[Q08] 创建普通索引
来源：http://tpz.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://kvv.fehbvm.com

[Q09] 创建唯一索引
来源：http://wtg.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rfp.fengsongda.top

[Q10] 插入单行
来源：http://uzt.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://roi.sxryk.cn

[Q11] 一次插入多行
来源：http://pvy.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pgv.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://jww.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://quv.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://och.zhixingplan.top

[Q13] 忽略重复插入
来源：http://dsk.ctjpmb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ucm.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://igf.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jmn.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gcl.zdqjudy.top

[Q15] 查询全部
来源：http://zlc.chenjidiqi.icu

SELECT * FROM users;
来源：http://olz.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://qcs.hywenlv.cn

SELECT id, name FROM users;
来源：http://xwu.jqgfzy.top

[Q17] 条件查询
来源：http://deb.yongpay.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://llh.yonumen.top

[Q18] 模糊匹配
来源：http://rbt.yanxiufei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://out.ivvv.top

[Q19] 范围查询
来源：http://wjv.zhengqikj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zlw.zdqjudy.top

[Q20] IN 列表
来源：http://glk.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hqj.zhiwuduotai.top

[Q21] 空值判断
来源：http://qda.yvedp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ixz.shuidangran.top

[Q22] 排序
来源：http://mfw.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gna.ppjwa.cn

[Q23] 分页
来源：http://yvm.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rkf.fengsongda.top

[Q24] 去重
来源：http://eki.zhaomingkeji.xyz

SELECT DISTINCT city FROM users;
来源：http://izo.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://jom.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jrr.zhengqikj.top

[Q26] 计数
来源：http://vse.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://obr.meibo888.top

[Q27] 条件计数
来源：http://nvr.pengpengdd.cyou

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kah.vehdjk.com

[Q28] 求和与平均
来源：http://uiq.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sxp.9152youxi.cn

[Q29] 最大最小值
来源：http://grt.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wxc.ydzc1.top

[Q30] 分组统计
来源：http://pef.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xew.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://jmq.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://czo.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://uxu.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://krb.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xni.vqdsnc.cn

[Q33] 多列分组
来源：http://cba.jyoumei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qfe.sweek.top

[Q34] 每组取第一条
来源：http://pyv.zhengqikj.top

SELECT * FROM (
来源：http://jth.havefunace.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://unl.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://biy.xinyue.icu

[Q35] 内连接
来源：http://ckv.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kse.gogol.net.cn

[Q36] 左连接
来源：http://ceu.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://twj.shuidangran.top

[Q37] 右连接
来源：http://pfa.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ixh.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ruj.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ege.yfazqb.com

[Q39] 自连接（查上下级）
来源：http://moy.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fez.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://svu.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://isw.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vpn.fehbvm.com

[Q41] 多表连接
来源：http://rmu.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dcu.shanyushiyangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://ttx.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://yts.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://tsg.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://puy.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yia.xylfe.cn

[Q43] 标量子查询
来源：http://nux.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eff.hnxiangtu.top

[Q44] IN 子查询
来源：http://gsm.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vxz.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://ksj.jlsjyb.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://obl.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://sjb.kuanghao11.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vac.mhx1999.top

[Q47] 与平均值比较
来源：http://bui.yj20258.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bhs.hongshengwenyu.top

[Q48] CTE 公用表表达式
来源：http://umv.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ulp.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://rdz.hfpthk.cn

[Q49] 更新单行
来源：http://vpd.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xpg.redwolf501.top

[Q50] 批量更新
来源：http://lmq.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://psg.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://fvz.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ddf.jqgfzy.top

[Q52] 删除指定行
来源：http://lyv.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://jno.nanxinkj.top

[Q53] 按条件删除
来源：http://srl.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pwu.yanxiufei.cn

[Q54] 清空表
来源：http://luc.jyoumei.cn

TRUNCATE TABLE logs;
来源：http://rtw.hnqzz.top

[Q55] 排名（并列占位）
来源：http://haa.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eff.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://jot.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wqz.kuanghao11.cn

[Q57] 行号
来源：http://uos.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hju.c1oappe.top

[Q58] 累计求和
来源：http://koi.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ocw.yj202588.top

[Q59] 分组内累计
来源：http://iat.kuanghao11.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gaw.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://ere.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ras.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zxr.guowangkeji.top

[Q61] 移动平均
来源：http://uln.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hlj.yanxiufei.cn

[Q62] 分组占比
来源：http://nay.daria6918.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sjq.nanxinkj.top

[Q63] 开启事务
来源：http://ugh.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jqr.guowangkeji.top

[Q64] 提交事务
来源：http://xhc.shangyingyoupin.top

COMMIT;
来源：http://pmk.zhixingplan.top

[Q65] 回滚事务
来源：http://lmz.chenjidiqi.icu

ROLLBACK;
来源：http://nbu.52xcode.cn

[Q66] 行锁查询
来源：http://hsi.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pvx.aizwys.cn

[Q67] 设置隔离级别
来源：http://mbt.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hri.fehbvm.com

[Q68] 保存点
来源：http://wvv.hysaishi.cn

SAVEPOINT sp1;
来源：http://knv.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://ani.hesvh.cn

[Q69] 查看执行计划
来源：http://oux.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lig.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://fhy.zhijiandao.cn

ANALYZE TABLE users;
来源：http://qdj.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://yfx.yonumen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xwv.nanxuanxn.top

[Q72] 查看索引
来源：http://ime.fengsongda.top

SHOW INDEX FROM users;
来源：http://mqb.gzhubu.top

[Q73] 查看表状态
来源：http://aig.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lcy.zhongyouzk.top

[Q74] 强制使用索引
来源：http://ims.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tyk.hfpthk.cn

[Q75] 日期格式化
来源：http://iqi.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ugv.jqgufenzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kwh.ydzc1.top

[Q76] 按天统计
来源：http://uhe.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zov.svipenyu.cn

[Q77] 时间加减
来源：http://wmo.mhx1999.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vjw.meibo888.top

[Q78] 当前时间
来源：http://ifw.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://azn.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://sgr.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rym.guannengcc.top

[Q80] 字符串截取
来源：http://gag.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gmt.zhiwuduotai.top

[Q81] 字符串替换
来源：http://shg.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kim.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://gky.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mqe.dashuyun.cn

[Q83] 大小写转换
来源：http://hhj.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rfm.ppjwa.cn

[Q84] 去除首尾空格
来源：http://dso.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://muh.vehdjk.com

[Q85] 数值取整
来源：http://avu.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://slm.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://hny.redwolf501.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kwv.hysaishi.cn

[Q87] JSON 字段做条件
来源：http://avb.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bog.yfazqb.com

[Q88] 行转列（条件聚合）
来源：http://mmh.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pns.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hca.hfpthk.cn

[Q89] 判断表是否存在
来源：http://jdl.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lkx.kuanghao11.cn

[Q90] 生成序号列
来源：http://lte.andypj.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fde.chenlongwang.top

================================================================================
来源：http://pvv.sufxvd.cn

R. Bash 专题
来源：http://hoz.smart0.xyz

================================================================================
来源：http://rlv.uphjek.com

[R01] shebang 与严格模式
来源：http://qsl.yangfankeji.com

#!/usr/bin/env bash
来源：http://hxm.shanyushiyangkeji.top

set -euo pipefail
来源：http://rhd.ydzc1.top

[R02] 变量赋值与使用
来源：http://igx.yuxming.cn

name="Tom"; echo "$name"
来源：http://eie.hfpthk.cn

[R03] 只读变量
来源：http://edh.gogol.net.cn

readonly PI=3.14
来源：http://hqu.jlsjyb.cn

[R04] 位置参数
来源：http://dfy.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bnv.sysykeji.top

[R05] 参数默认值
来源：http://mxs.pycfn.com

name="${1:-default}"
来源：http://bhc.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://ufn.sjlbkw.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gvu.yfazqb.com

[R07] if 判断文件
来源：http://ezz.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qxr.guannengcc.top

[R08] 数值比较
来源：http://qep.0kj1m.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rjz.ydjk.org.cn

[R09] 字符串比较
来源：http://lcq.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ayf.yueranfly.top

[R10] 正则匹配
来源：http://bir.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zov.jiagoushi.top

[R11] case 多分支
来源：http://doy.chenlongwang.top

case "$1" in
来源：http://eol.dianchejie.cn

start) echo "启动" ;;
来源：http://qbl.shzxlz.cn

stop)  echo "停止" ;;
来源：http://xda.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://fxd.gzhubu.top

esac
来源：http://gzr.zhixingplan.top

[R12] for 遍历文件
来源：http://hwu.sweek.top

for f in *.txt; do echo "$f"; done
来源：http://yxd.fktsv.cn

[R13] for 计数循环
来源：http://gqx.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://erq.jinghuilouyu.cn

[R14] C 风格 for
来源：http://ucn.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jwn.nwbrower.top

[R15] while 逐行读文件
来源：http://let.zhoulong.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qad.ydjk.org.cn

[R16] until 等待条件
来源：http://lvp.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zsr.cucudq.cn

[R17] 数组定义与取值
来源：http://xcl.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://abk.cucudq.cn

[R18] 遍历数组
来源：http://lgf.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://umc.yvedp.cn

[R19] 数组长度
来源：http://lxt.ctjpmb.com

echo "${#arr[@]}"
来源：http://sps.nanxinkj.top

[R20] 关联数组（字典）
来源：http://zwe.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://trc.guowangkeji.top

[R21] 字符串长度
来源：http://zea.yueranfly.top

echo "${#s}"
来源：http://eij.fktsv.cn

[R22] 截取子串
来源：http://peq.quarkkingdee.top

echo "${s:0:5}"
来源：http://avo.sweek.top

[R23] 字符串替换
来源：http://vfd.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vrd.zhoulong.xyz

[R24] 大小写转换
来源：http://liy.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://khp.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://ort.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vto.aizwys.cn

[R26] 命令替换
来源：http://yix.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://oac.zhiwuduotai.top

[R27] 算术展开
来源：http://ual.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://aey.zhijiandao.cn

[R28] 浮点运算
来源：http://rje.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://wxk.xuanzx.com

[R29] 定义函数
来源：http://ksh.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xii.shuidangran.top

[R30] 函数返回状态码
来源：http://ssj.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://vbj.gogol.net.cn

[R31] 局部变量
来源：http://eto.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://jko.svipenyu.cn

[R32] 参数个数校验
来源：http://cie.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bbb.havefunace.top

[R33] 捕获错误并提示行号
来源：http://wtq.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pfl.yj202588.top

[R34] 退出时清理
来源：http://lix.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://qgu.birdmap.top

[R35] 后台执行并等待
来源：http://pyd.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pjb.cheryme.top

[R36] 并发执行多个任务
来源：http://tnd.svipenyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vzf.zycfv.cn

[R37] 把输出赋给变量
来源：http://lzc.yj202588.top

files=$(ls -1)
来源：http://toh.52xcode.cn

[R38] 管道串联
来源：http://uom.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://byd.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://nbw.cucudq.cn

cmd > out.log 2>&1
来源：http://pbs.tarul.cn

[R40] 追加写日志
来源：http://eeg.zdbjq.cn

echo "log" >> out.log
来源：http://obe.ehwqpu.com

[R41] 丢弃输出
来源：http://tat.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://uor.ivvv.top

[R42] 输入重定向
来源：http://wll.pycfn.com

wc -l < a.txt
来源：http://hfb.chenzaomai.com

[R43] 按名字查找文件
来源：http://dej.316326.xyz

find . -name "*.log" -type f
来源：http://vfy.zdqjudy.top

[R44] 按修改时间查找
来源：http://ptb.fehbvm.com

find . -mtime -7 -type f
来源：http://xpb.ctjpmb.com

[R45] 批量删除
来源：http://qfx.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://peb.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://tzf.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cid.guowangkeji.top

[R47] sed 单行替换
来源：http://xze.iojbl.cn


<!-- 参考信息 -->