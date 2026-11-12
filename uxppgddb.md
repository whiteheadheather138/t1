代发 wailian999

CREATE TABLE users (
来源：http://ebd.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ohd.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://gdx.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://zsb.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eig.daxiang520.top

);
来源：http://xox.shangyingyoupin.top

[Q02] 创建带外键的表
来源：http://btr.cheryme.top

CREATE TABLE orders (
来源：http://sqi.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://usw.ydjk.org.cn

user_id INT NOT NULL,
来源：http://ouo.hongshengwenyu.top

amount DECIMAL(10, 2),
来源：http://tca.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hoe.dianchejie.cn

);
来源：http://rct.zycfv.cn

[Q03] 增加列
来源：http://onf.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zdo.zhijiandao.cn

[Q04] 修改列类型
来源：http://nzq.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://usk.jqgfzy.top

[Q05] 重命名列
来源：http://oyq.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://guj.fanxiaobao.xyz

[Q06] 删除列
来源：http://qdz.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://ojq.52xcode.cn

[Q07] 删除表
来源：http://adp.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://qru.ctjpmb.com

[Q08] 创建普通索引
来源：http://jky.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xjj.zhijiandao.cn

[Q09] 创建唯一索引
来源：http://wuo.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qxi.kuanghao11.cn

[Q10] 插入单行
来源：http://lqv.cashguo.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eqa.ydzc1.top

[Q11] 一次插入多行
来源：http://jud.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://akz.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://gvt.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://hkp.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ily.gzhubu.top

[Q13] 忽略重复插入
来源：http://xrk.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oey.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://udz.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qmr.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ppe.chenzaomai.com

[Q15] 查询全部
来源：http://axn.yvedp.cn

SELECT * FROM users;
来源：http://zbl.yuxming.cn

[Q16] 查询指定列
来源：http://myl.gzhubu.top

SELECT id, name FROM users;
来源：http://bdp.guannengcc.top

[Q17] 条件查询
来源：http://rbn.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kpe.chenlongwang.top

[Q18] 模糊匹配
来源：http://nfc.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dry.zhiwuduotai.top

[Q19] 范围查询
来源：http://lzg.vehdjk.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://szw.yonumen.top

[Q20] IN 列表
来源：http://fjr.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://emb.0kj1m.cn

[Q21] 空值判断
来源：http://hyj.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kcg.snrcjt.cn

[Q22] 排序
来源：http://vaq.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gws.ctjpmb.com

[Q23] 分页
来源：http://txs.yj20258888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jwt.jqgfzy.top

[Q24] 去重
来源：http://obb.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://slp.ehwqpu.com

[Q25] 只取前 N 条
来源：http://fhi.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nja.sxryk.cn

[Q26] 计数
来源：http://oss.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://yyk.hfpthk.cn

[Q27] 条件计数
来源：http://rde.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ltd.ctjpmb.com

[Q28] 求和与平均
来源：http://xhd.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rvn.guannengcc.top

[Q29] 最大最小值
来源：http://elx.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vpw.tianlin.xyz

[Q30] 分组统计
来源：http://fxh.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ijb.chenlongwang.top

[Q31] 分组后过滤
来源：http://hea.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tts.bjfxy.top

[Q32] 分组拼接字符串
来源：http://agq.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wta.cashguo.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dxx.guowangkeji.top

[Q33] 多列分组
来源：http://ejo.9152youxi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gvx.shzxlz.cn

[Q34] 每组取第一条
来源：http://rxm.ctjpmb.com

SELECT * FROM (
来源：http://enl.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hnc.zycfv.cn

) t WHERE rn = 1;
来源：http://ftx.chenjidiqi.icu

[Q35] 内连接
来源：http://air.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kju.gotoacloud.top

[Q36] 左连接
来源：http://lug.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cul.shangyingyoupin.top

[Q37] 右连接
来源：http://nxv.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hfx.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://knr.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uwj.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://kak.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ano.dashuyun.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eoc.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jcf.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fny.sjlbkw.cn

[Q41] 多表连接
来源：http://yej.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kgm.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://tdk.ehwqpu.com

JOIN products p ON p.id = o.product_id;
来源：http://yyw.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://lev.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://bxl.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yvc.jinqigufen.top

[Q43] 标量子查询
来源：http://ypq.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uys.pycfn.com

[Q44] IN 子查询
来源：http://dmp.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ekc.c1oappe.top

[Q45] EXISTS 判断存在
来源：http://eoq.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fri.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://kjc.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mzd.smart0.xyz

[Q47] 与平均值比较
来源：http://qvm.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jkh.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://bpm.sweek.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hdr.chenjidiqi.icu

SELECT * FROM t WHERE c > 5;
来源：http://wrp.pycfn.com

[Q49] 更新单行
来源：http://kfi.fanxiaobao.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fao.vqdsnc.cn

[Q50] 批量更新
来源：http://jsf.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kxa.52xcode.cn

[Q51] 用子查询更新
来源：http://sjg.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bmb.quarkkingdee.top

[Q52] 删除指定行
来源：http://eug.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://vcw.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://xwf.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qrs.cashguo.top

[Q54] 清空表
来源：http://qbp.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://mhf.c1oappe.top

[Q55] 排名（并列占位）
来源：http://bdq.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oxm.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://rpr.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oyh.xziqi.cn

[Q57] 行号
来源：http://qdi.vehdjk.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zfs.guowangkeji.top

[Q58] 累计求和
来源：http://ehz.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mht.sysykeji.top

[Q59] 分组内累计
来源：http://ale.yongpay.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jpq.sysykeji.top

[Q60] 取上一行 / 下一行
来源：http://rso.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ppd.hesvh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://whv.sweek.top

[Q61] 移动平均
来源：http://feu.0kj1m.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aaa.redwolf501.top

[Q62] 分组占比
来源：http://khz.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xkk.ivvv.top

[Q63] 开启事务
来源：http://abx.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wwh.shanyushiyangtech.top

[Q64] 提交事务
来源：http://wws.tanke756.top

COMMIT;
来源：http://rcm.bjfxy.top

[Q65] 回滚事务
来源：http://lle.yangfankeji.com

ROLLBACK;
来源：http://neu.yfazqb.com

[Q66] 行锁查询
来源：http://gme.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lze.wangdashe.top

[Q67] 设置隔离级别
来源：http://ipb.vehdjk.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gys.yj202588.top

[Q68] 保存点
来源：http://cqs.hcnkem.com

SAVEPOINT sp1;
来源：http://vja.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://bgl.ivvv.top

[Q69] 查看执行计划
来源：http://mus.jinqigufen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tfk.redwolf501.top

[Q70] 更新统计信息
来源：http://bla.sxryk.cn

ANALYZE TABLE users;
来源：http://kxm.bjfxy.top

[Q71] 查看建表语句
来源：http://uaq.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zdq.wangshuangyany.cn

[Q72] 查看索引
来源：http://rlr.hywenlv.cn

SHOW INDEX FROM users;
来源：http://gys.svipenyu.cn

[Q73] 查看表状态
来源：http://aat.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ssk.iojbl.cn

[Q74] 强制使用索引
来源：http://hgz.tanke756.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dgu.nwbrower.top

[Q75] 日期格式化
来源：http://vfd.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tae.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dck.hammf.cn

[Q76] 按天统计
来源：http://ziw.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lqa.fehbvm.com

[Q77] 时间加减
来源：http://ezk.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ood.hongshengwenyu.top

[Q78] 当前时间
来源：http://sdi.epnwcf.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mln.feifeiyinyue.top

[Q79] 字符串拼接
来源：http://bcz.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zyc.gogol.net.cn

[Q80] 字符串截取
来源：http://yje.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hcr.shangyingyoupin.top

[Q81] 字符串替换
来源：http://krs.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hwv.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://mwu.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bnf.xuetiantiany.cn

[Q83] 大小写转换
来源：http://szp.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://chh.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://xqm.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://utp.zhaomingkeji.xyz

[Q85] 数值取整
来源：http://klu.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://haf.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://swn.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xfd.fehbvm.com

[Q87] JSON 字段做条件
来源：http://kuh.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kka.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://gqm.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aso.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wvi.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://bfp.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ubx.gzhubu.top

[Q90] 生成序号列
来源：http://mvz.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yvj.jqgfzy.top

================================================================================
来源：http://shm.zhoulong.xyz

R. Bash 专题
来源：http://yim.cucudq.cn

================================================================================
来源：http://fpj.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://era.sweek.top

#!/usr/bin/env bash
来源：http://nyd.fehbvm.com

set -euo pipefail
来源：http://fnm.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://lri.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://idt.hysaishi.cn

[R03] 只读变量
来源：http://wdu.feifeiyinyue.top

readonly PI=3.14
来源：http://epw.smart0.xyz

[R04] 位置参数
来源：http://ift.vqdsnc.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aow.pycfn.com

[R05] 参数默认值
来源：http://nqt.yanxiufei.cn

name="${1:-default}"
来源：http://mqx.ctjpmb.com

[R06] 判断命令是否存在
来源：http://aew.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zdk.ydjk.org.cn

[R07] if 判断文件
来源：http://ysi.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dup.zdbjq.cn

[R08] 数值比较
来源：http://dke.haohaochexian.top

if (( a > b )); then echo "a 更大"; fi
来源：http://msv.xuetiantiany.cn

[R09] 字符串比较
来源：http://mbn.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fwr.jqgfzy.top

[R10] 正则匹配
来源：http://rzp.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nsr.tanke756.top

[R11] case 多分支
来源：http://gya.yuanzhike.top

case "$1" in
来源：http://edn.ehwqpu.com

start) echo "启动" ;;
来源：http://wxx.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://dsm.yj202588.top

*)     echo "未知命令" ;;
来源：http://okt.hongshengwenyu.top

esac
来源：http://wez.yj20258888.top

[R12] for 遍历文件
来源：http://xbc.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://jiv.yj20258.top

[R13] for 计数循环
来源：http://eof.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://elp.hesvh.cn

[R14] C 风格 for
来源：http://kze.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://siu.hnxiangtu.top

[R15] while 逐行读文件
来源：http://pya.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mzh.gotoacloud.top

[R16] until 等待条件
来源：http://unm.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ssh.nanxuanxn.top

[R17] 数组定义与取值
来源：http://nqm.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jdf.zycfv.cn

[R18] 遍历数组
来源：http://lvj.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ryc.kuanghao11.cn

[R19] 数组长度
来源：http://lxw.ppjwa.cn

echo "${#arr[@]}"
来源：http://mkd.daxiang520.top

[R20] 关联数组（字典）
来源：http://aes.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ikl.zhengqikj.top

[R21] 字符串长度
来源：http://atr.yfazqb.com

echo "${#s}"
来源：http://xrb.snrcjt.cn

[R22] 截取子串
来源：http://quq.zdbjq.cn

echo "${s:0:5}"
来源：http://blx.smart0.xyz

[R23] 字符串替换
来源：http://nru.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zbo.zycfv.cn

[R24] 大小写转换
来源：http://fkw.zhoulong.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://bsy.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://wzd.pycfn.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://xkf.0kj1m.cn

[R26] 命令替换
来源：http://zad.cqqwz.cn

now=$(date +%F); echo "$now"
来源：http://ffc.haohaochexian.top

[R27] 算术展开
来源：http://sxd.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://usr.zhijiandao.cn

[R28] 浮点运算
来源：http://lpp.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://tqy.cucudq.cn

[R29] 定义函数
来源：http://tyg.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jud.ydzc1.top

[R30] 函数返回状态码
来源：http://svv.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://uzk.zhongyouzk.top

[R31] 局部变量
来源：http://yod.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://wtf.gzhubu.top

[R32] 参数个数校验
来源：http://qpm.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rgt.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://vun.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://psq.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://dgg.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rru.wangdashe.top

[R35] 后台执行并等待
来源：http://ybx.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ilc.nanxinkj.top

[R36] 并发执行多个任务
来源：http://pep.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ksx.yj202588.top

[R37] 把输出赋给变量
来源：http://pxm.zhijiandao.cn

files=$(ls -1)
来源：http://bzs.pengpengdd.cyou

[R38] 管道串联
来源：http://ois.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://dcf.yonumen.top

[R39] 重定向标准输出与错误
来源：http://bhz.ppjwa.cn

cmd > out.log 2>&1
来源：http://wbm.cqqwz.cn

[R40] 追加写日志
来源：http://fsi.nanxinkj.top

echo "log" >> out.log
来源：http://yjq.wangdashe.top

[R41] 丢弃输出
来源：http://gsk.cqqwz.cn

cmd >/dev/null 2>&1
来源：http://whm.xuanzx.com

[R42] 输入重定向
来源：http://qnb.jyoumei.cn

wc -l < a.txt
来源：http://nax.cucudq.cn

[R43] 按名字查找文件
来源：http://dev.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://pwm.fzhhl.top

[R44] 按修改时间查找
来源：http://sfn.cashguo.top

find . -mtime -7 -type f
来源：http://xio.yj20258888.top

[R45] 批量删除
来源：http://zur.quarkkingdee.top


<!-- 参考信息 -->