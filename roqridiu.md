代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvc.bjfxy.top

user_id INT NOT NULL,
来源：http://jhe.fehbvm.com

amount DECIMAL(10, 2),
来源：http://bvc.fanxiaobao.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://akz.havefunace.top

);
来源：http://kfg.ehwqpu.com

[Q03] 增加列
来源：http://jkx.yangfankeji.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qip.haohaochexian.top

[Q04] 修改列类型
来源：http://ohi.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hsk.gogol.net.cn

[Q05] 重命名列
来源：http://eop.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fzt.gogol.net.cn

[Q06] 删除列
来源：http://zru.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qnm.zhengqikj.top

[Q07] 删除表
来源：http://oat.cdnleiting.top

DROP TABLE IF EXISTS orders;
来源：http://iek.kuanghao11.cn

[Q08] 创建普通索引
来源：http://bkv.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rhm.zdqjudy.top

[Q09] 创建唯一索引
来源：http://ktz.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://beu.jqgfzy.top

[Q10] 插入单行
来源：http://ooo.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uof.dashuyun.cn

[Q11] 一次插入多行
来源：http://zwd.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ern.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://abm.vehdjk.com

INSERT INTO users (name) VALUES ('C');
来源：http://dwy.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sdo.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://ryz.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://crh.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://jip.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://grl.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://soy.shzxlz.cn

[Q15] 查询全部
来源：http://hap.fktsv.cn

SELECT * FROM users;
来源：http://tbz.jianghu66.top

[Q16] 查询指定列
来源：http://xcj.c1oappe.top

SELECT id, name FROM users;
来源：http://thf.xinyue.icu

[Q17] 条件查询
来源：http://ctq.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wzy.yueranfly.top

[Q18] 模糊匹配
来源：http://ruv.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ovw.c1oappe.top

[Q19] 范围查询
来源：http://bbd.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://epq.tian-w.cn

[Q20] IN 列表
来源：http://wbm.dianchejie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kws.snrcjt.cn

[Q21] 空值判断
来源：http://fzq.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://etf.zhengqikj.top

[Q22] 排序
来源：http://soq.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://swj.zycfv.cn

[Q23] 分页
来源：http://ynp.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://svo.shanyushiyangkeji.top

[Q24] 去重
来源：http://hcw.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://nit.hywenlv.cn

[Q25] 只取前 N 条
来源：http://icq.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uaj.aizwys.cn

[Q26] 计数
来源：http://ykq.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://brd.bjfxy.top

[Q27] 条件计数
来源：http://llq.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yii.yvedp.cn

[Q28] 求和与平均
来源：http://hak.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://boc.wangshuangyany.cn

[Q29] 最大最小值
来源：http://pfw.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sbh.aizwys.cn

[Q30] 分组统计
来源：http://vej.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://caq.316326.xyz

[Q31] 分组后过滤
来源：http://qrf.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://exu.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://ybk.redwolf501.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://idp.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aln.tianlin.xyz

[Q33] 多列分组
来源：http://cgu.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hum.ppjwa.cn

[Q34] 每组取第一条
来源：http://wcz.jyoumei.cn

SELECT * FROM (
来源：http://fej.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://quz.zycfv.cn

) t WHERE rn = 1;
来源：http://fpn.gaohongyu789.top

[Q35] 内连接
来源：http://yyo.fehbvm.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uov.0kj1m.cn

[Q36] 左连接
来源：http://qtu.dianchejie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nap.316326.xyz

[Q37] 右连接
来源：http://drs.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ujl.jyoumei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nhd.quarkkingdee.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xmz.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://brv.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://byy.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://egc.tianlin.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://gfz.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jzf.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://lxw.gzhubu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zci.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://scb.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://mod.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://beb.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://vpj.birdmap.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jyf.ehwqpu.com

[Q43] 标量子查询
来源：http://kst.bjfxy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lbk.vehdjk.com

[Q44] IN 子查询
来源：http://pji.ppjwa.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wpc.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://xsv.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ruh.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://wtl.birdmap.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://isc.yanxiufei.cn

[Q47] 与平均值比较
来源：http://giy.hfpthk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://byw.cqqwz.cn

[Q48] CTE 公用表表达式
来源：http://izl.zhaomingkeji.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dmc.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://gbn.jinqigfzy.top

[Q49] 更新单行
来源：http://cmi.jyoumei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xee.zdbjq.cn

[Q50] 批量更新
来源：http://flg.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dzy.iojbl.cn

[Q51] 用子查询更新
来源：http://xqk.epnwcf.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ndb.c1oappe.top

[Q52] 删除指定行
来源：http://zyi.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://nfv.cheryme.top

[Q53] 按条件删除
来源：http://gmz.fanxiaobao.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lch.52xcode.cn

[Q54] 清空表
来源：http://wyi.ppjwa.cn

TRUNCATE TABLE logs;
来源：http://qpa.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://emg.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ttv.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://shl.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rdx.dashuyun.cn

[Q57] 行号
来源：http://hbu.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ujn.smart0.xyz

[Q58] 累计求和
来源：http://jtn.shuidangran.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qpg.xziqi.cn

[Q59] 分组内累计
来源：http://bas.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gnv.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://alk.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ghd.yj20258888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vfo.zdbjq.cn

[Q61] 移动平均
来源：http://dbs.dianchejie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qnv.guowangkeji.top

[Q62] 分组占比
来源：http://gbh.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cnt.hysaishi.cn

[Q63] 开启事务
来源：http://aqq.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://hve.ctjpmb.com

[Q64] 提交事务
来源：http://zue.guannengcc.top

COMMIT;
来源：http://jdh.xylfe.cn

[Q65] 回滚事务
来源：http://mas.epnwcf.com

ROLLBACK;
来源：http://cni.gaohongyu789.top

[Q66] 行锁查询
来源：http://kry.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://duv.uphjek.com

[Q67] 设置隔离级别
来源：http://uga.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fam.uphjek.com

[Q68] 保存点
来源：http://qmy.jianghu66.top

SAVEPOINT sp1;
来源：http://yqg.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://gdy.epnwcf.com

[Q69] 查看执行计划
来源：http://teh.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vih.fehbvm.com

[Q70] 更新统计信息
来源：http://ejm.guannengcc.top

ANALYZE TABLE users;
来源：http://sfd.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://mma.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ajm.pengpengdd.cyou

[Q72] 查看索引
来源：http://wjl.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://dni.xuetiantiany.cn

[Q73] 查看表状态
来源：http://tbm.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iqs.yonumen.top

[Q74] 强制使用索引
来源：http://tvz.mhx1999.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fss.sufxvd.cn

[Q75] 日期格式化
来源：http://qbv.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xux.zhoulong.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fot.jinghuilouyu.cn

[Q76] 按天统计
来源：http://wji.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hff.tianlin.xyz

[Q77] 时间加减
来源：http://pxh.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hez.gaohongyu789.top

[Q78] 当前时间
来源：http://njg.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qxf.hcnkem.com

[Q79] 字符串拼接
来源：http://rvq.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kpd.vehdjk.com

[Q80] 字符串截取
来源：http://gxp.zhiwuduotai.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ymy.havefunace.top

[Q81] 字符串替换
来源：http://tzb.xziqi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gzl.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://ekm.sxryk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://geo.guowangkeji.top

[Q83] 大小写转换
来源：http://jts.aibaodan.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mki.guannengcc.top

[Q84] 去除首尾空格
来源：http://lmi.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://kps.quarkkingdee.top

[Q85] 数值取整
来源：http://vvv.chenzaomai.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://trr.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://mcl.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zoh.mhx1999.top

[Q87] JSON 字段做条件
来源：http://aew.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ghs.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://bfk.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lka.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iru.ydzc1.top

[Q89] 判断表是否存在
来源：http://kyb.gotoacloud.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wpd.kuanghao11.cn

[Q90] 生成序号列
来源：http://gjn.ywan-chungtsiang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yak.jyoumei.cn

================================================================================
来源：http://lfu.pengpengdd.cyou

R. Bash 专题
来源：http://wgt.zhixingplan.top

================================================================================
来源：http://evo.nanxinkj.top

[R01] shebang 与严格模式
来源：http://jge.jinqigufen.top

#!/usr/bin/env bash
来源：http://ppn.cashguo.top

set -euo pipefail
来源：http://vmg.quarkkingdee.top

[R02] 变量赋值与使用
来源：http://tnu.fengsongda.top

name="Tom"; echo "$name"
来源：http://qfg.wangdashe.top

[R03] 只读变量
来源：http://ysm.316326.xyz

readonly PI=3.14
来源：http://zlo.cheryme.top

[R04] 位置参数
来源：http://loq.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ome.ehwqpu.com

[R05] 参数默认值
来源：http://nmn.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://eix.yvedp.cn

[R06] 判断命令是否存在
来源：http://kwt.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lut.yj20258.top

[R07] if 判断文件
来源：http://mos.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ikh.hongshengwenyu.top

[R08] 数值比较
来源：http://isi.9152youxi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yfj.zycfv.cn

[R09] 字符串比较
来源：http://fzf.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lni.dashuyun.cn

[R10] 正则匹配
来源：http://unu.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mve.yj202588.top

[R11] case 多分支
来源：http://cgm.hcnkem.com

case "$1" in
来源：http://hgx.yvedp.cn

start) echo "启动" ;;
来源：http://zbf.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://nwg.andypj.xyz

*)     echo "未知命令" ;;
来源：http://vak.xuanzx.com

esac
来源：http://byz.zhiwuduotai.top

[R12] for 遍历文件
来源：http://gjs.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://kxd.yj20258888.top

[R13] for 计数循环
来源：http://tfy.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://kar.316326.xyz

[R14] C 风格 for
来源：http://ykn.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sye.andypj.xyz

[R15] while 逐行读文件
来源：http://scu.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ooa.jinghuilouyu.cn

[R16] until 等待条件
来源：http://udf.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dku.xylfe.cn

[R17] 数组定义与取值
来源：http://mdx.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://auh.quarkkingdee.top

[R18] 遍历数组
来源：http://tck.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vbd.vehdjk.com

[R19] 数组长度
来源：http://fra.chenzaomai.com

echo "${#arr[@]}"
来源：http://rpe.dashuyun.cn

[R20] 关联数组（字典）
来源：http://zow.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lsq.jlsjyb.cn

[R21] 字符串长度
来源：http://tel.xuanzx.com

echo "${#s}"
来源：http://aqu.jiagoushi.top

[R22] 截取子串
来源：http://rgx.zhiwuduotai.top

echo "${s:0:5}"
来源：http://utf.zhongyouzk.top

[R23] 字符串替换
来源：http://jki.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oka.cheryme.top

[R24] 大小写转换
来源：http://exc.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://oyu.yongpay.top

[R25] 去后缀 / 去前缀
来源：http://xpp.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://los.0kj1m.cn

[R26] 命令替换
来源：http://qku.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://pdq.zhaomingkeji.xyz

[R27] 算术展开
来源：http://qcw.hnqzz.top

echo $((1 + 2 * 3))
来源：http://vdq.jinyuanbaomall.cn

[R28] 浮点运算
来源：http://ueb.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://kej.fanxiaobao.xyz

[R29] 定义函数
来源：http://upe.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lzf.zhixingplan.top

[R30] 函数返回状态码
来源：http://kqu.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://mro.zhaomingkeji.xyz

[R31] 局部变量
来源：http://fci.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://znn.feifeiyinyue.top

[R32] 参数个数校验
来源：http://onb.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://liz.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://jst.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bqp.sysykeji.top

[R34] 退出时清理
来源：http://dxj.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://ifo.ctjpmb.com

[R35] 后台执行并等待
来源：http://xbt.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ylp.yongpay.top

[R36] 并发执行多个任务
来源：http://bzb.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vsd.ivvv.top

[R37] 把输出赋给变量
来源：http://xsm.ydjk.org.cn

files=$(ls -1)
来源：http://fwg.gogol.net.cn

[R38] 管道串联
来源：http://wbu.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://kks.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://xeb.yonumen.top

cmd > out.log 2>&1
来源：http://jgr.vqdsnc.cn

[R40] 追加写日志
来源：http://vsv.gaohongyu789.top

echo "log" >> out.log
来源：http://tcd.nanxinkj.top

[R41] 丢弃输出
来源：http://qbz.c1oappe.top

cmd >/dev/null 2>&1
来源：http://hsg.wangshuangyany.cn

[R42] 输入重定向
来源：http://jzw.ybcxt.top

wc -l < a.txt
来源：http://fxc.sufxvd.cn

[R43] 按名字查找文件
来源：http://bfg.jianghu66.top

find . -name "*.log" -type f
来源：http://mky.dashuyun.cn

[R44] 按修改时间查找
来源：http://zwb.xziqi.cn

find . -mtime -7 -type f
来源：http://bgf.zhaomingkeji.xyz

[R45] 批量删除
来源：http://uqk.tanke756.top

find . -name "*.tmp" -delete
来源：http://bev.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://rpf.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gfe.ydjk.org.cn

[R47] sed 单行替换
来源：http://qze.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://lzf.jqgufenzy.top

[R48] awk 取指定列
来源：http://wpo.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://ube.cheryme.top

[R49] awk 带条件
来源：http://ero.shzxlz.cn


<!-- 参考信息 -->