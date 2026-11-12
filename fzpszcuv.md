代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zhi.gzhubu.top

user_id INT NOT NULL,
来源：http://orj.fzhhl.top

amount DECIMAL(10, 2),
来源：http://ibf.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://txy.nanxinkj.top

);
来源：http://gcr.hfpthk.cn

[Q03] 增加列
来源：http://tkf.hysaishi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tta.jqgufenzy.top

[Q04] 修改列类型
来源：http://bgq.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sfr.pengpengdd.cyou

[Q05] 重命名列
来源：http://wmg.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wuh.chenjidiqi.icu

[Q06] 删除列
来源：http://jip.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ipf.tarul.cn

[Q07] 删除表
来源：http://faz.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://tqn.sysykeji.top

[Q08] 创建普通索引
来源：http://vfm.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://flu.sxryk.cn

[Q09] 创建唯一索引
来源：http://eod.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ejd.chenzaomai.com

[Q10] 插入单行
来源：http://lxz.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://khm.chenjidiqi.icu

[Q11] 一次插入多行
来源：http://ojl.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lfb.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://dke.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://fdr.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vzt.nwbrower.top

[Q13] 忽略重复插入
来源：http://eno.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://swg.sxryk.cn

[Q14] 存在则更新（upsert）
来源：http://vbk.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zey.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lpq.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://hjz.chenlongwang.top

SELECT * FROM users;
来源：http://iqf.dashuyun.cn

[Q16] 查询指定列
来源：http://fut.gogol.net.cn

SELECT id, name FROM users;
来源：http://kep.ydzc1.top

[Q17] 条件查询
来源：http://wsh.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uyi.daria6918.cn

[Q18] 模糊匹配
来源：http://ilq.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://glh.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://ige.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qkp.zdqjudy.top

[Q20] IN 列表
来源：http://ndu.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xvf.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://bqn.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bsh.daria6918.cn

[Q22] 排序
来源：http://wcp.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zpq.pycfn.com

[Q23] 分页
来源：http://gyy.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cpb.jinghuilouyu.cn

[Q24] 去重
来源：http://mil.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://cae.yvedp.cn

[Q25] 只取前 N 条
来源：http://wtq.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://drs.daria6918.cn

[Q26] 计数
来源：http://wro.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://fqq.52xcode.cn

[Q27] 条件计数
来源：http://rrp.jinghuilouyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jfx.tian-w.cn

[Q28] 求和与平均
来源：http://msu.cdnleiting.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://src.zdbjq.cn

[Q29] 最大最小值
来源：http://idd.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hwq.yj20258888.top

[Q30] 分组统计
来源：http://kmp.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vqh.mhx1999.top

[Q31] 分组后过滤
来源：http://gao.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zrg.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://imc.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uzg.tanke756.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fah.tianlin.xyz

[Q33] 多列分组
来源：http://xah.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zkc.jiagoushi.top

[Q34] 每组取第一条
来源：http://qmx.dashuyun.cn

SELECT * FROM (
来源：http://uun.hywenlv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cmc.tarul.cn

) t WHERE rn = 1;
来源：http://uct.hammf.cn

[Q35] 内连接
来源：http://pfv.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://swf.chenlongwang.top

[Q36] 左连接
来源：http://gze.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ykx.havefunace.top

[Q37] 右连接
来源：http://die.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oqd.hesvh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cpj.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ehf.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://maw.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yhr.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mqg.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ysk.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mwk.cucudq.cn

[Q41] 多表连接
来源：http://qur.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ncl.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://vlf.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://yfm.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://xqh.smart0.xyz

SELECT u.name, o.amount FROM users u
来源：http://kcp.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ctp.epnwcf.com

[Q43] 标量子查询
来源：http://tou.fanxiaobao.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kum.zhengqikj.top

[Q44] IN 子查询
来源：http://hlb.cashguo.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wdm.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://rmn.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oup.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://ska.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://isa.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://cqd.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ntk.cqqwz.cn

[Q48] CTE 公用表表达式
来源：http://tzr.ppjwa.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ybf.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://fhv.jyoumei.cn

[Q49] 更新单行
来源：http://btr.kuanghao11.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kab.yj20258.top

[Q50] 批量更新
来源：http://hvd.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eiw.dianchejie.cn

[Q51] 用子查询更新
来源：http://ahr.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wma.chenlongwang.top

[Q52] 删除指定行
来源：http://msq.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://igp.gzhubu.top

[Q53] 按条件删除
来源：http://irr.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zmg.pycfn.com

[Q54] 清空表
来源：http://grv.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://rjq.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://tfm.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aph.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://wmc.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zzm.shanyushiyangkeji.top

[Q57] 行号
来源：http://nci.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uql.zhaomingkeji.xyz

[Q58] 累计求和
来源：http://yqd.kuanghao11.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kbp.nanxuanxn.top

[Q59] 分组内累计
来源：http://jos.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xls.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://yhv.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ixi.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jun.xinyue.icu

[Q61] 移动平均
来源：http://gwi.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qfm.hnxiangtu.top

[Q62] 分组占比
来源：http://qxq.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yfw.ivvv.top

[Q63] 开启事务
来源：http://ook.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://srd.snrcjt.cn

[Q64] 提交事务
来源：http://rkd.zdqjudy.top

COMMIT;
来源：http://ucv.yuanzhike.top

[Q65] 回滚事务
来源：http://aok.sxryk.cn

ROLLBACK;
来源：http://rpf.sysykeji.top

[Q66] 行锁查询
来源：http://bjf.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qha.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://sim.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tgu.nwbrower.top

[Q68] 保存点
来源：http://noc.zhaomingkeji.xyz

SAVEPOINT sp1;
来源：http://znk.ywan-chungtsiang.top

ROLLBACK TO sp1;
来源：http://lbz.xingfuxueyuan.xyz

[Q69] 查看执行计划
来源：http://xmi.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://duo.jinqigufen.top

[Q70] 更新统计信息
来源：http://xju.yangfankeji.com

ANALYZE TABLE users;
来源：http://xfs.dianchejie.cn

[Q71] 查看建表语句
来源：http://nlj.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://djg.xziqi.cn

[Q72] 查看索引
来源：http://jbh.birdmap.top

SHOW INDEX FROM users;
来源：http://gjz.yanxiufei.cn

[Q73] 查看表状态
来源：http://uuj.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tpk.ydzc1.top

[Q74] 强制使用索引
来源：http://zzc.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kua.guannengcc.top

[Q75] 日期格式化
来源：http://gwl.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xqq.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dvd.aizwys.cn

[Q76] 按天统计
来源：http://uvg.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nnr.pycfn.com

[Q77] 时间加减
来源：http://itq.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vwk.tian-w.cn

[Q78] 当前时间
来源：http://lrk.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uac.nwbrower.top

[Q79] 字符串拼接
来源：http://fgo.gogol.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://txg.andypj.xyz

[Q80] 字符串截取
来源：http://siq.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://egr.sufxvd.cn

[Q81] 字符串替换
来源：http://uwh.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://naw.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://mhk.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uph.smart0.xyz

[Q83] 大小写转换
来源：http://yxo.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://abn.9152youxi.cn

[Q84] 去除首尾空格
来源：http://ldg.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://dxr.gogol.net.cn

[Q85] 数值取整
来源：http://pmr.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uss.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://ghx.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aym.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://iay.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lnx.yj202588.top

[Q88] 行转列（条件聚合）
来源：http://hng.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pex.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://miy.zhoulong.xyz

[Q89] 判断表是否存在
来源：http://xgm.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zls.zhijiandao.cn

[Q90] 生成序号列
来源：http://xct.ywan-chungtsiang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://emf.cdnleiting.top

================================================================================
来源：http://cxw.zhongyouzk.top

R. Bash 专题
来源：http://kvw.hesvh.cn

================================================================================
来源：http://dun.yongpay.top

[R01] shebang 与严格模式
来源：http://qdp.zycfv.cn

#!/usr/bin/env bash
来源：http://utj.iojbl.cn

set -euo pipefail
来源：http://whw.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://fih.fktsv.cn

name="Tom"; echo "$name"
来源：http://pto.cucudq.cn

[R03] 只读变量
来源：http://xlj.316326.xyz

readonly PI=3.14
来源：http://hqs.svipenyu.cn

[R04] 位置参数
来源：http://hwl.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ppa.zycfv.cn

[R05] 参数默认值
来源：http://hih.daxiang520.top

name="${1:-default}"
来源：http://mkk.ybcxt.top

[R06] 判断命令是否存在
来源：http://afy.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rmq.fktsv.cn

[R07] if 判断文件
来源：http://hmh.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kil.ctjpmb.com

[R08] 数值比较
来源：http://ldw.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://xdi.52xcode.cn

[R09] 字符串比较
来源：http://qza.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kcm.chenlongwang.top

[R10] 正则匹配
来源：http://tmq.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cmc.zhijiandao.cn

[R11] case 多分支
来源：http://vgw.hammf.cn

case "$1" in
来源：http://nrq.jqgfzy.top

start) echo "启动" ;;
来源：http://zfk.shzxlz.cn

stop)  echo "停止" ;;
来源：http://xly.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://ucm.yongpay.top

esac
来源：http://phk.gotoacloud.top

[R12] for 遍历文件
来源：http://cep.xziqi.cn

for f in *.txt; do echo "$f"; done
来源：http://drv.shangyingyoupin.top

[R13] for 计数循环
来源：http://gny.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://ggu.zycfv.cn

[R14] C 风格 for
来源：http://tdz.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gna.quarkkingdee.top

[R15] while 逐行读文件
来源：http://khe.smart0.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://btw.tanke756.top

[R16] until 等待条件
来源：http://gdi.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jtx.cashguo.top

[R17] 数组定义与取值
来源：http://hjq.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://ylc.pycfn.com

[R18] 遍历数组
来源：http://fne.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gfl.xinyue.icu

[R19] 数组长度
来源：http://amk.ppjwa.cn

echo "${#arr[@]}"
来源：http://bye.zycfv.cn

[R20] 关联数组（字典）
来源：http://kxz.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qkj.hfpthk.cn

[R21] 字符串长度
来源：http://tul.xuetiantiany.cn

echo "${#s}"
来源：http://zmj.jinyuanbaomall.cn

[R22] 截取子串
来源：http://hhx.ehwqpu.com

echo "${s:0:5}"
来源：http://kvn.yj20258.top

[R23] 字符串替换
来源：http://wtt.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nnb.yj20258.top

[R24] 大小写转换
来源：http://zhj.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://une.ydzc1.top

[R25] 去后缀 / 去前缀
来源：http://lgr.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://scs.jinyuanbaomall.cn

[R26] 命令替换
来源：http://vrn.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://opj.yongpay.top

[R27] 算术展开
来源：http://bwj.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://iiq.yj20258.top

[R28] 浮点运算
来源：http://qmt.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://nmz.yj20258888.top

[R29] 定义函数
来源：http://xdw.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aid.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://ufr.hammf.cn

f() { return 0; }; f || echo "失败了"
来源：http://vac.yj202588.top

[R31] 局部变量
来源：http://qyx.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://rpn.yfazqb.com

[R32] 参数个数校验
来源：http://omv.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://snk.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://ctt.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lng.fktsv.cn

[R34] 退出时清理
来源：http://olv.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://drb.zdqjudy.top

[R35] 后台执行并等待
来源：http://yse.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dxh.bjfxy.top

[R36] 并发执行多个任务
来源：http://nnk.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ahp.tian-w.cn

[R37] 把输出赋给变量
来源：http://brb.0kj1m.cn

files=$(ls -1)
来源：http://osp.yj20258888.top

[R38] 管道串联
来源：http://gxr.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://yxk.tanke756.top

[R39] 重定向标准输出与错误
来源：http://zzq.yj202588.top

cmd > out.log 2>&1
来源：http://wan.zhixingplan.top

[R40] 追加写日志
来源：http://ogo.tarul.cn

echo "log" >> out.log
来源：http://ejc.52xcode.cn

[R41] 丢弃输出
来源：http://kga.sxryk.cn

cmd >/dev/null 2>&1
来源：http://cnf.hongshengwenyu.top

[R42] 输入重定向
来源：http://kdh.iojbl.cn

wc -l < a.txt
来源：http://tlp.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://zaq.cdnleiting.top

find . -name "*.log" -type f
来源：http://lcm.daria6918.cn

[R44] 按修改时间查找
来源：http://zcp.kuanghao11.cn

find . -mtime -7 -type f
来源：http://cuh.meibo888.top

[R45] 批量删除
来源：http://dza.smart0.xyz

find . -name "*.tmp" -delete
来源：http://hyb.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://mvj.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vfj.0kj1m.cn

[R47] sed 单行替换
来源：http://dpx.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://qeu.yj20258888.top

[R48] awk 取指定列
来源：http://nxm.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://ljy.hfpthk.cn

[R49] awk 带条件
来源：http://kqx.jlsjyb.cn


<!-- 参考信息 -->