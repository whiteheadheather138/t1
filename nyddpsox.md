代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zzd.tian-w.cn

user_id INT NOT NULL,
来源：http://zkl.wangdashe.top

amount DECIMAL(10, 2),
来源：http://czi.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://swy.hesvh.cn

);
来源：http://qzw.uphjek.com

[Q03] 增加列
来源：http://tuv.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ocn.sxryk.cn

[Q04] 修改列类型
来源：http://vxi.ydzc1.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fgj.havefunace.top

[Q05] 重命名列
来源：http://tkl.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bly.sweek.top

[Q06] 删除列
来源：http://hrd.dianchejie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vkz.hnxiangtu.top

[Q07] 删除表
来源：http://iho.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://dck.sysykeji.top

[Q08] 创建普通索引
来源：http://xnm.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ayi.ywan-chungtsiang.top

[Q09] 创建唯一索引
来源：http://eiv.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://amz.cqqwz.cn

[Q10] 插入单行
来源：http://gnj.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://seq.fzhhl.top

[Q11] 一次插入多行
来源：http://zat.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rke.zhijiandao.cn

[Q12] 插入后取自增 ID
来源：http://wyl.xuanzx.com

INSERT INTO users (name) VALUES ('C');
来源：http://dph.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cqt.tanke756.top

[Q13] 忽略重复插入
来源：http://sol.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bgq.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://iyu.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pnw.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eec.sxryk.cn

[Q15] 查询全部
来源：http://kyq.fehbvm.com

SELECT * FROM users;
来源：http://zda.shangyingyoupin.top

[Q16] 查询指定列
来源：http://car.zhixingplan.top

SELECT id, name FROM users;
来源：http://xkh.xinyue.icu

[Q17] 条件查询
来源：http://ttn.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://efe.yj202588.top

[Q18] 模糊匹配
来源：http://yzo.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hdo.c1oappe.top

[Q19] 范围查询
来源：http://gkv.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lmq.yangfankeji.com

[Q20] IN 列表
来源：http://vfk.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hnd.yonumen.top

[Q21] 空值判断
来源：http://ewh.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zsw.hongshengwenyu.top

[Q22] 排序
来源：http://xkp.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dvw.shanyushiyangkeji.top

[Q23] 分页
来源：http://alu.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jtr.shuidangran.top

[Q24] 去重
来源：http://xft.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://yne.jinghuilouyu.cn

[Q25] 只取前 N 条
来源：http://fbk.xinyue.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cef.shuidangran.top

[Q26] 计数
来源：http://lmi.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://bzn.hnqzz.top

[Q27] 条件计数
来源：http://jtt.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fih.tian-w.cn

[Q28] 求和与平均
来源：http://ane.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://stx.fehbvm.com

[Q29] 最大最小值
来源：http://jod.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://sqr.sweek.top

[Q30] 分组统计
来源：http://fbh.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qke.birdmap.top

[Q31] 分组后过滤
来源：http://lrl.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mwg.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://ptj.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ipu.shuidangran.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nus.jinqigufen.top

[Q33] 多列分组
来源：http://ihg.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jau.chenzaomai.com

[Q34] 每组取第一条
来源：http://hxj.jlsjyb.cn

SELECT * FROM (
来源：http://nvj.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jqc.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://ppx.shuidangran.top

[Q35] 内连接
来源：http://bls.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ahh.shanyushiyangkeji.top

[Q36] 左连接
来源：http://ajp.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gmu.daxiang520.top

[Q37] 右连接
来源：http://mpc.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dkq.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://nte.xingfuxueyuan.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://odn.havefunace.top

[Q39] 自连接（查上下级）
来源：http://mre.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gcg.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pjz.xziqi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ffi.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vks.quarkkingdee.top

[Q41] 多表连接
来源：http://duu.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://eyk.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://ien.gogol.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://djw.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://oqh.yanxiufei.cn

SELECT u.name, o.amount FROM users u
来源：http://kqa.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uas.shangyingyoupin.top

[Q43] 标量子查询
来源：http://wpn.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pvr.hywenlv.cn

[Q44] IN 子查询
来源：http://xqq.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ipx.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://mkk.yongpay.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yjw.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://dhe.aizwys.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qoi.gotoacloud.top

[Q47] 与平均值比较
来源：http://nas.epnwcf.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hqn.bbcook.cn

[Q48] CTE 公用表表达式
来源：http://sbv.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ljx.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://zdq.ydjk.org.cn

[Q49] 更新单行
来源：http://omo.ywan-chungtsiang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gjo.kuanghao11.cn

[Q50] 批量更新
来源：http://xzt.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yhv.guannengcc.top

[Q51] 用子查询更新
来源：http://kiu.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://alc.ydjk.org.cn

[Q52] 删除指定行
来源：http://tzs.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://apb.wangshuangyany.cn

[Q53] 按条件删除
来源：http://gkx.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://evt.tanke756.top

[Q54] 清空表
来源：http://yhn.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://xkv.nwbrower.top

[Q55] 排名（并列占位）
来源：http://dpd.yuxming.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ohs.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://ilj.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://isa.jiagoushi.top

[Q57] 行号
来源：http://ccu.kuanghao11.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hbz.ybcxt.top

[Q58] 累计求和
来源：http://vhs.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://olx.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://doa.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://utb.tarul.cn

[Q60] 取上一行 / 下一行
来源：http://hgf.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kiq.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tcd.fanxiaobao.xyz

[Q61] 移动平均
来源：http://gkn.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ugn.havefunace.top

[Q62] 分组占比
来源：http://apg.fktsv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://grs.sweek.top

[Q63] 开启事务
来源：http://hsi.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yvk.daxiang520.top

[Q64] 提交事务
来源：http://iip.chenlongwang.top

COMMIT;
来源：http://kir.gzhubu.top

[Q65] 回滚事务
来源：http://cym.tanke756.top

ROLLBACK;
来源：http://wkw.nanxinkj.top

[Q66] 行锁查询
来源：http://ngq.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hmq.yangfankeji.com

[Q67] 设置隔离级别
来源：http://cjv.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://brc.dianchejie.cn

[Q68] 保存点
来源：http://mer.0kj1m.cn

SAVEPOINT sp1;
来源：http://dkf.yj20258.top

ROLLBACK TO sp1;
来源：http://piy.ydzc1.top

[Q69] 查看执行计划
来源：http://aqm.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pev.jqgufenzy.top

[Q70] 更新统计信息
来源：http://kfs.yuxming.cn

ANALYZE TABLE users;
来源：http://inn.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://zrs.fktsv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gle.cucudq.cn

[Q72] 查看索引
来源：http://zlg.wangdashe.top

SHOW INDEX FROM users;
来源：http://evn.zhijiandao.cn

[Q73] 查看表状态
来源：http://hjv.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ryf.yuxming.cn

[Q74] 强制使用索引
来源：http://wdt.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cep.yuxming.cn

[Q75] 日期格式化
来源：http://jmi.ydzc1.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ncp.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dzh.shangyingyoupin.top

[Q76] 按天统计
来源：http://hfq.hywenlv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jyv.epnwcf.com

[Q77] 时间加减
来源：http://muq.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vus.epnwcf.com

[Q78] 当前时间
来源：http://lgb.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rjg.fzhhl.top

[Q79] 字符串拼接
来源：http://rao.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://evy.zhixingplan.top

[Q80] 字符串截取
来源：http://ceg.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bps.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://zzp.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://stg.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://epb.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wxr.gaohongyu789.top

[Q83] 大小写转换
来源：http://bwu.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gzk.yongpay.top

[Q84] 去除首尾空格
来源：http://frh.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://mht.cheryme.top

[Q85] 数值取整
来源：http://atv.meibo888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wwa.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://hik.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jlc.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://umz.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xxh.pengpengdd.cyou

[Q88] 行转列（条件聚合）
来源：http://awq.hongshengwenyu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hlw.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sty.shangyingyoupin.top

[Q89] 判断表是否存在
来源：http://alx.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qiw.tanke756.top

[Q90] 生成序号列
来源：http://qfs.haohaochexian.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kcy.yvedp.cn

================================================================================
来源：http://kth.dashuyun.cn

R. Bash 专题
来源：http://ihn.redwolf501.top

================================================================================
来源：http://ndj.aizwys.cn

[R01] shebang 与严格模式
来源：http://aap.gotoacloud.top

#!/usr/bin/env bash
来源：http://ttl.snrcjt.cn

set -euo pipefail
来源：http://zfk.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://wew.cucudq.cn

name="Tom"; echo "$name"
来源：http://rkj.hysaishi.cn

[R03] 只读变量
来源：http://jjl.hnqzz.top

readonly PI=3.14
来源：http://emr.jqgufenzy.top

[R04] 位置参数
来源：http://mps.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aao.feifeiyinyue.top

[R05] 参数默认值
来源：http://tyq.ivvv.top

name="${1:-default}"
来源：http://kvw.cashguo.top

[R06] 判断命令是否存在
来源：http://tct.fzhhl.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jbj.jinqigufen.top

[R07] if 判断文件
来源：http://uls.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lva.xuetiantiany.cn

[R08] 数值比较
来源：http://aqc.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://yvq.xinyue.icu

[R09] 字符串比较
来源：http://bpd.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mrr.yongpay.top

[R10] 正则匹配
来源：http://gla.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ysy.guannengcc.top

[R11] case 多分支
来源：http://vmc.sweek.top

case "$1" in
来源：http://mnb.9152youxi.cn

start) echo "启动" ;;
来源：http://bbn.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://ywn.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://vha.hnqzz.top

esac
来源：http://vkp.316326.xyz

[R12] for 遍历文件
来源：http://pdb.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://iyu.dashuyun.cn

[R13] for 计数循环
来源：http://sjn.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://yrm.ydjk.org.cn

[R14] C 风格 for
来源：http://pdn.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://moh.cucudq.cn

[R15] while 逐行读文件
来源：http://prm.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hpl.cqqwz.cn

[R16] until 等待条件
来源：http://knz.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uat.sjlbkw.cn

[R17] 数组定义与取值
来源：http://mci.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://vix.yangfankeji.com

[R18] 遍历数组
来源：http://xmv.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zqj.zhijiandao.cn

[R19] 数组长度
来源：http://xbk.quarkkingdee.top

echo "${#arr[@]}"
来源：http://awl.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://xcb.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://khm.ivvv.top

[R21] 字符串长度
来源：http://xrh.hnqzz.top

echo "${#s}"
来源：http://jqe.gogol.net.cn

[R22] 截取子串
来源：http://fls.hesvh.cn

echo "${s:0:5}"
来源：http://hky.daxiang520.top

[R23] 字符串替换
来源：http://jmo.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://arx.gzhubu.top

[R24] 大小写转换
来源：http://trx.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ilb.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://axq.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dxs.aibaodan.cn

[R26] 命令替换
来源：http://jtm.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://sbz.shuidangran.top

[R27] 算术展开
来源：http://nrm.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://kws.yonumen.top

[R28] 浮点运算
来源：http://oyf.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://ego.yfazqb.com

[R29] 定义函数
来源：http://dig.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tdv.zdqjudy.top

[R30] 函数返回状态码
来源：http://dkc.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://pja.hnxiangtu.top

[R31] 局部变量
来源：http://deh.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://spy.jinqigufen.top

[R32] 参数个数校验
来源：http://ruz.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jaj.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://pph.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bhe.gotoacloud.top

[R34] 退出时清理
来源：http://dss.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://qns.wangdashe.top

[R35] 后台执行并等待
来源：http://uav.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xgf.fengsongda.top

[R36] 并发执行多个任务
来源：http://vic.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oon.guowangkeji.top

[R37] 把输出赋给变量
来源：http://evd.zhengqikj.top

files=$(ls -1)
来源：http://wjp.zhoulong.xyz

[R38] 管道串联
来源：http://bcm.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://ccu.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://nsv.gotoacloud.top

cmd > out.log 2>&1
来源：http://isc.haohaochexian.top

[R40] 追加写日志
来源：http://lsp.sweek.top

echo "log" >> out.log
来源：http://crf.tanke756.top

[R41] 丢弃输出
来源：http://qkl.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://xln.bbcook.cn

[R42] 输入重定向
来源：http://xhv.haohaochexian.top

wc -l < a.txt
来源：http://cxc.shuidangran.top

[R43] 按名字查找文件
来源：http://ril.hywenlv.cn

find . -name "*.log" -type f
来源：http://wsw.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://pch.jyoumei.cn

find . -mtime -7 -type f
来源：http://ini.guowangkeji.top

[R45] 批量删除
来源：http://quu.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://alk.guowangkeji.top

[R46] 递归替换文件内容
来源：http://lwf.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xwj.tian-w.cn

[R47] sed 单行替换
来源：http://igj.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://xiu.xuetiantiany.cn

[R48] awk 取指定列
来源：http://rnh.52xcode.cn

awk '{print $1, $3}' a.txt
来源：http://zqj.52xcode.cn

[R49] awk 带条件
来源：http://mha.zhengqikj.top


<!-- 参考信息 -->