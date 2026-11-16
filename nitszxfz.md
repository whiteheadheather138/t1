代发 wailian999

================================================================================
来源：http://hxr.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vpo.hesvh.cn

================================================================================
来源：http://bnn.52xcode.cn

[Q01] 创建表
来源：http://hxr.chenjidiqi.icu

CREATE TABLE users (
来源：http://zyr.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sav.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://qrg.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://uga.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lrp.yj20258888.top

);
来源：http://vwq.gogol.net.cn

[Q02] 创建带外键的表
来源：http://xpf.xylfe.cn

CREATE TABLE orders (
来源：http://ngl.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://okt.hywenlv.cn

user_id INT NOT NULL,
来源：http://cre.hongshengwenyu.top

amount DECIMAL(10, 2),
来源：http://mqc.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rod.dianchejie.cn

);
来源：http://hfw.chenlongwang.top

[Q03] 增加列
来源：http://mij.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yuz.zdbjq.cn

[Q04] 修改列类型
来源：http://klf.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://exp.wangshuangyany.cn

[Q05] 重命名列
来源：http://lay.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://axc.zhengqikj.top

[Q06] 删除列
来源：http://fai.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://axc.redwolf501.top

[Q07] 删除表
来源：http://fxs.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://zfw.hywenlv.cn

[Q08] 创建普通索引
来源：http://utk.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bnr.vehdjk.com

[Q09] 创建唯一索引
来源：http://oxe.feifeiyinyue.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bvi.birdmap.top

[Q10] 插入单行
来源：http://rii.jqgfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://icf.daria6918.cn

[Q11] 一次插入多行
来源：http://bcr.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pxm.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://nio.jianghu66.top

INSERT INTO users (name) VALUES ('C');
来源：http://lvs.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xxn.ppjwa.cn

[Q13] 忽略重复插入
来源：http://mwc.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xqg.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://joq.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iou.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://usz.jianghu66.top

[Q15] 查询全部
来源：http://zib.zhoulong.xyz

SELECT * FROM users;
来源：http://fin.yuanzhike.top

[Q16] 查询指定列
来源：http://uje.ctjpmb.com

SELECT id, name FROM users;
来源：http://uxx.ydzc1.top

[Q17] 条件查询
来源：http://etk.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tom.jinqigfzy.top

[Q18] 模糊匹配
来源：http://yli.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hvh.bjfxy.top

[Q19] 范围查询
来源：http://fvh.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://frd.0kj1m.cn

[Q20] IN 列表
来源：http://yuc.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pai.yj20258888.top

[Q21] 空值判断
来源：http://sdr.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qph.sufxvd.cn

[Q22] 排序
来源：http://wus.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tjv.gaohongyu789.top

[Q23] 分页
来源：http://ysz.daria6918.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ffj.jlsjyb.cn

[Q24] 去重
来源：http://pzn.gogol.net.cn

SELECT DISTINCT city FROM users;
来源：http://ver.yuxming.cn

[Q25] 只取前 N 条
来源：http://pyy.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dvq.hysaishi.cn

[Q26] 计数
来源：http://xro.xziqi.cn

SELECT COUNT(*) FROM users;
来源：http://exp.yvedp.cn

[Q27] 条件计数
来源：http://jzi.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dzh.daria6918.cn

[Q28] 求和与平均
来源：http://tvr.hesvh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://evz.mhx1999.top

[Q29] 最大最小值
来源：http://dlf.wangdashe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qic.ivvv.top

[Q30] 分组统计
来源：http://dbf.shzxlz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sml.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://jsh.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rgu.xinyue.icu

[Q32] 分组拼接字符串
来源：http://awt.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://czt.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kuj.sweek.top

[Q33] 多列分组
来源：http://ctz.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mpm.gotoacloud.top

[Q34] 每组取第一条
来源：http://ppl.guowangkeji.top

SELECT * FROM (
来源：http://pyr.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dyn.tianlin.xyz

) t WHERE rn = 1;
来源：http://bug.zhiwuduotai.top

[Q35] 内连接
来源：http://vki.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qnz.xinyue.icu

[Q36] 左连接
来源：http://tfd.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gxv.svipenyu.cn

[Q37] 右连接
来源：http://piv.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rid.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://exy.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pjd.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://qan.guowangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tvm.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vxg.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lvw.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dzi.hywenlv.cn

[Q41] 多表连接
来源：http://vac.hnqzz.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wnz.dianchejie.cn

JOIN users u ON u.id = o.user_id
来源：http://tpe.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://zja.guannengcc.top

[Q42] 连接条件附加过滤
来源：http://pem.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://bkr.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nfc.quarkkingdee.top

[Q43] 标量子查询
来源：http://xhv.zhijiandao.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://msg.pycfn.com

[Q44] IN 子查询
来源：http://aje.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oip.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://ota.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bou.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yjx.ivvv.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://olu.hammf.cn

[Q47] 与平均值比较
来源：http://ikz.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yfy.birdmap.top

[Q48] CTE 公用表表达式
来源：http://hph.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rbc.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://izw.aizwys.cn

[Q49] 更新单行
来源：http://mjo.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oxc.pycfn.com

[Q50] 批量更新
来源：http://kpn.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://psg.aizwys.cn

[Q51] 用子查询更新
来源：http://uif.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fdu.yuanzhike.top

[Q52] 删除指定行
来源：http://xeq.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://qgt.pycfn.com

[Q53] 按条件删除
来源：http://mpv.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jrc.zhiwuduotai.top

[Q54] 清空表
来源：http://rtb.hnqzz.top

TRUNCATE TABLE logs;
来源：http://dom.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://fro.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gke.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://thy.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rqx.cqqwz.cn

[Q57] 行号
来源：http://odv.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vax.ctjpmb.com

[Q58] 累计求和
来源：http://qgr.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://asi.wangdashe.top

[Q59] 分组内累计
来源：http://dtt.pengpengdd.cyou

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nzz.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://igx.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wtz.xziqi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vbh.fehbvm.com

[Q61] 移动平均
来源：http://ftz.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vqw.jlsjyb.cn

[Q62] 分组占比
来源：http://hyq.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vqn.shzxlz.cn

[Q63] 开启事务
来源：http://orh.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nvh.dianchejie.cn

[Q64] 提交事务
来源：http://stq.guannengcc.top

COMMIT;
来源：http://ese.zdbjq.cn

[Q65] 回滚事务
来源：http://ysu.sufxvd.cn

ROLLBACK;
来源：http://ikf.jqgfzy.top

[Q66] 行锁查询
来源：http://eom.dashuyun.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zxe.0kj1m.cn

[Q67] 设置隔离级别
来源：http://nny.jinqigufen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zmn.hywenlv.cn

[Q68] 保存点
来源：http://srl.yfazqb.com

SAVEPOINT sp1;
来源：http://ilz.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://dax.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://hrc.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qjw.jyoumei.cn

[Q70] 更新统计信息
来源：http://zxy.zhiwuduotai.top

ANALYZE TABLE users;
来源：http://tlf.gotoacloud.top

[Q71] 查看建表语句
来源：http://xeh.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xfe.zhixingplan.top

[Q72] 查看索引
来源：http://uiv.zhiwuduotai.top

SHOW INDEX FROM users;
来源：http://luy.tarul.cn

[Q73] 查看表状态
来源：http://bbp.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sgg.cucudq.cn

[Q74] 强制使用索引
来源：http://rtb.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bty.fzhhl.top

[Q75] 日期格式化
来源：http://knb.ybcxt.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://quq.hcnkem.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qca.snrcjt.cn

[Q76] 按天统计
来源：http://nyu.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ucf.zycfv.cn

[Q77] 时间加减
来源：http://mvi.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tzu.chenjidiqi.icu

[Q78] 当前时间
来源：http://osk.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mmg.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://cog.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cct.tianlin.xyz

[Q80] 字符串截取
来源：http://uli.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gdg.sysykeji.top

[Q81] 字符串替换
来源：http://bcr.hfpthk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wnx.tanke756.top

[Q82] 字符长度与字节长度
来源：http://etx.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://arf.zhongyouzk.top

[Q83] 大小写转换
来源：http://lil.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wyk.dashuyun.cn

[Q84] 去除首尾空格
来源：http://iwg.fehbvm.com

SELECT TRIM(name) FROM users;
来源：http://alt.cucudq.cn

[Q85] 数值取整
来源：http://izq.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bag.316326.xyz

[Q86] 读取 JSON 字段
来源：http://saw.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dau.iojbl.cn

[Q87] JSON 字段做条件
来源：http://jlj.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://klx.0kj1m.cn

[Q88] 行转列（条件聚合）
来源：http://ssi.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lyt.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vye.guannengcc.top

[Q89] 判断表是否存在
来源：http://dpl.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jlx.hywenlv.cn

[Q90] 生成序号列
来源：http://mxx.yuanzhike.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fnk.daxiang520.top

================================================================================
来源：http://vzc.zdbjq.cn

R. Bash 专题
来源：http://mcp.quarkkingdee.top

================================================================================
来源：http://xfe.shzxlz.cn

[R01] shebang 与严格模式
来源：http://ukl.bbcook.cn

#!/usr/bin/env bash
来源：http://xej.chenzaomai.com

set -euo pipefail
来源：http://nvr.0kj1m.cn

[R02] 变量赋值与使用
来源：http://tvt.ivvv.top

name="Tom"; echo "$name"
来源：http://kpf.yueranfly.top

[R03] 只读变量
来源：http://bul.yanxiufei.cn

readonly PI=3.14
来源：http://caj.hysaishi.cn

[R04] 位置参数
来源：http://efg.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jsj.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://eir.vehdjk.com

name="${1:-default}"
来源：http://tci.tianlin.xyz

[R06] 判断命令是否存在
来源：http://pwh.svipenyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lri.aibaodan.cn

[R07] if 判断文件
来源：http://cng.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ieu.sweek.top

[R08] 数值比较
来源：http://kwi.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dzw.sysykeji.top

[R09] 字符串比较
来源：http://tkr.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fbc.shangyingyoupin.top

[R10] 正则匹配
来源：http://nue.shanyushiyangtech.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ofu.nanxinkj.top

[R11] case 多分支
来源：http://efy.xylfe.cn

case "$1" in
来源：http://eaq.cqqwz.cn

start) echo "启动" ;;
来源：http://pzf.zhixingplan.top

stop)  echo "停止" ;;
来源：http://hxb.ydzc1.top

*)     echo "未知命令" ;;
来源：http://yos.52xcode.cn

esac
来源：http://teb.birdmap.top

[R12] for 遍历文件
来源：http://tdu.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://zbl.guannengcc.top

[R13] for 计数循环
来源：http://scr.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://dxl.zhiwuduotai.top

[R14] C 风格 for
来源：http://rjv.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://spk.mhx1999.top

[R15] while 逐行读文件
来源：http://pyr.havefunace.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wkf.smart0.xyz

[R16] until 等待条件
来源：http://ria.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://and.shuidangran.top

[R17] 数组定义与取值
来源：http://fli.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jky.meibo888.top

[R18] 遍历数组
来源：http://qud.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hre.jqgfzy.top

[R19] 数组长度
来源：http://fgi.iojbl.cn

echo "${#arr[@]}"
来源：http://vfi.haohaochexian.top

[R20] 关联数组（字典）
来源：http://qln.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eyd.yuanzhike.top

[R21] 字符串长度
来源：http://huf.sjlbkw.cn

echo "${#s}"
来源：http://pdl.havefunace.top

[R22] 截取子串
来源：http://hgd.pengpengdd.cyou

echo "${s:0:5}"
来源：http://wio.haohaochexian.top

[R23] 字符串替换
来源：http://jjf.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qex.cucudq.cn

[R24] 大小写转换
来源：http://xii.hesvh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fkc.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://tsp.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://nxi.chenlongwang.top

[R26] 命令替换
来源：http://ejt.tianlin.xyz

now=$(date +%F); echo "$now"
来源：http://pax.zhixingplan.top

[R27] 算术展开
来源：http://swh.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://fen.wangdashe.top

[R28] 浮点运算
来源：http://wsg.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://ycw.9152youxi.cn

[R29] 定义函数
来源：http://dey.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yjf.jiagoushi.top

[R30] 函数返回状态码
来源：http://fds.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://pvx.shangyingyoupin.top

[R31] 局部变量
来源：http://weu.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://kzh.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://pcl.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pqo.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://guu.fengsongda.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wmr.zdqjudy.top

[R34] 退出时清理
来源：http://xot.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://sfp.fzhhl.top

[R35] 后台执行并等待
来源：http://upl.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ped.gogol.net.cn

[R36] 并发执行多个任务
来源：http://kpo.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vpx.snrcjt.cn

[R37] 把输出赋给变量
来源：http://kdx.uphjek.com

files=$(ls -1)
来源：http://ryd.tian-w.cn

[R38] 管道串联
来源：http://ejn.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://dqd.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://dwx.smart0.xyz

cmd > out.log 2>&1
来源：http://blv.mhx1999.top

[R40] 追加写日志
来源：http://yvu.ydzc1.top

echo "log" >> out.log
来源：http://rmf.yongpay.top

[R41] 丢弃输出
来源：http://qeu.yonumen.top

cmd >/dev/null 2>&1
来源：http://dhs.quarkkingdee.top

[R42] 输入重定向
来源：http://qpu.tian-w.cn

wc -l < a.txt
来源：http://oqe.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://mps.xziqi.cn


<!-- 参考信息 -->