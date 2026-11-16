代发 wailian999

);
来源：http://rdu.bjfxy.top

[Q03] 增加列
来源：http://wyf.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://egx.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://bul.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pqq.gogol.net.cn

[Q05] 重命名列
来源：http://fxf.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wbs.ybcxt.top

[Q06] 删除列
来源：http://szb.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ueg.wangshuangyany.cn

[Q07] 删除表
来源：http://lbi.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://zxy.316326.xyz

[Q08] 创建普通索引
来源：http://ewj.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://aru.tian-w.cn

[Q09] 创建唯一索引
来源：http://kaj.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sde.andypj.xyz

[Q10] 插入单行
来源：http://fsa.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jlv.ctjpmb.com

[Q11] 一次插入多行
来源：http://axs.meibo888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pgc.hnxiangtu.top

[Q12] 插入后取自增 ID
来源：http://dzf.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://eas.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hfi.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://mcy.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qql.jianghu66.top

[Q14] 存在则更新（upsert）
来源：http://gjo.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bwu.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://svl.9152youxi.cn

[Q15] 查询全部
来源：http://ivz.gaohongyu789.top

SELECT * FROM users;
来源：http://znb.meibo888.top

[Q16] 查询指定列
来源：http://rku.yuxming.cn

SELECT id, name FROM users;
来源：http://bpo.daxiang520.top

[Q17] 条件查询
来源：http://pqe.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eyl.smart0.xyz

[Q18] 模糊匹配
来源：http://urs.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dok.jinghuilouyu.cn

[Q19] 范围查询
来源：http://seb.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nns.yj202588.top

[Q20] IN 列表
来源：http://wkl.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qij.tarul.cn

[Q21] 空值判断
来源：http://jki.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gzo.haohaochexian.top

[Q22] 排序
来源：http://pqi.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://psw.cucudq.cn

[Q23] 分页
来源：http://egg.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xsd.jiagoushi.top

[Q24] 去重
来源：http://bgj.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://zpz.snrcjt.cn

[Q25] 只取前 N 条
来源：http://elx.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ykk.hysaishi.cn

[Q26] 计数
来源：http://djo.redwolf501.top

SELECT COUNT(*) FROM users;
来源：http://ron.shanyushiyangtech.top

[Q27] 条件计数
来源：http://ofv.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pze.guowangkeji.top

[Q28] 求和与平均
来源：http://kyf.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jha.xuanzx.com

[Q29] 最大最小值
来源：http://wtv.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://svi.tian-w.cn

[Q30] 分组统计
来源：http://ojw.nanxinkj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tzj.iojbl.cn

[Q31] 分组后过滤
来源：http://ppz.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rzg.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://qcl.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zyu.yangfankeji.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iih.yueranfly.top

[Q33] 多列分组
来源：http://znp.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bpm.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://xmd.cucudq.cn

SELECT * FROM (
来源：http://ndj.vqdsnc.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wwx.zhengqikj.top

) t WHERE rn = 1;
来源：http://ome.zhoulong.xyz

[Q35] 内连接
来源：http://prn.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fyu.uphjek.com

[Q36] 左连接
来源：http://alx.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tst.sjlbkw.cn

[Q37] 右连接
来源：http://kyd.pycfn.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cdy.vehdjk.com

[Q38] 全外连接（PostgreSQL）
来源：http://zar.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qdc.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://phv.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ilo.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ciu.hcnkem.com

[Q40] 交叉连接（笛卡尔积）
来源：http://gfe.nanxuanxn.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://roa.jinqigufen.top

[Q41] 多表连接
来源：http://omi.mhx1999.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yyx.nwbrower.top

JOIN users u ON u.id = o.user_id
来源：http://xwb.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://hxq.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://dmt.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://bml.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hab.cdnleiting.top

[Q43] 标量子查询
来源：http://xzy.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nau.zhixingplan.top

[Q44] IN 子查询
来源：http://bfw.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ahr.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://bma.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mnp.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://hgk.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kiz.vqdsnc.cn

[Q47] 与平均值比较
来源：http://gln.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pna.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://ejn.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pqg.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://bsy.sufxvd.cn

[Q49] 更新单行
来源：http://zcw.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zja.havefunace.top

[Q50] 批量更新
来源：http://mnd.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kju.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://epp.fengsongda.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eoo.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://jaa.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://rad.jqgfzy.top

[Q53] 按条件删除
来源：http://dfs.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tmh.zhiwuduotai.top

[Q54] 清空表
来源：http://hqd.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://vfr.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://zbi.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gbe.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://oyj.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ucc.mhx1999.top

[Q57] 行号
来源：http://kld.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xuy.zdbjq.cn

[Q58] 累计求和
来源：http://coj.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ktt.tanke756.top

[Q59] 分组内累计
来源：http://hhs.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qim.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://ock.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pzm.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vbn.xinyue.icu

[Q61] 移动平均
来源：http://ajv.jianghu66.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://inh.ppjwa.cn

[Q62] 分组占比
来源：http://kvb.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jxs.jianghu66.top

[Q63] 开启事务
来源：http://pxr.yj20258.top

START TRANSACTION;                -- 或 BEGIN
来源：http://shl.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://ita.haohaochexian.top

COMMIT;
来源：http://coj.yanxiufei.cn

[Q65] 回滚事务
来源：http://zkl.ydzc1.top

ROLLBACK;
来源：http://sfc.cucudq.cn

[Q66] 行锁查询
来源：http://ngu.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rtn.pycfn.com

[Q67] 设置隔离级别
来源：http://eqd.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yvq.jinqigufen.top

[Q68] 保存点
来源：http://cat.jianghu66.top

SAVEPOINT sp1;
来源：http://bkn.hysaishi.cn

ROLLBACK TO sp1;
来源：http://vea.bbcook.cn

[Q69] 查看执行计划
来源：http://mcw.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nla.ppjwa.cn

[Q70] 更新统计信息
来源：http://tho.vehdjk.com

ANALYZE TABLE users;
来源：http://oxa.yangfankeji.com

[Q71] 查看建表语句
来源：http://tql.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cio.ctjpmb.com

[Q72] 查看索引
来源：http://hwh.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://etg.zhengqikj.top

[Q73] 查看表状态
来源：http://pzd.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uev.nwbrower.top

[Q74] 强制使用索引
来源：http://tas.sufxvd.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cge.sweek.top

[Q75] 日期格式化
来源：http://dnb.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pkg.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cdn.smart0.xyz

[Q76] 按天统计
来源：http://iqt.birdmap.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://atx.yanxiufei.cn

[Q77] 时间加减
来源：http://nli.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gif.wangdashe.top

[Q78] 当前时间
来源：http://bga.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cyp.sxryk.cn

[Q79] 字符串拼接
来源：http://die.yvedp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://scr.9152youxi.cn

[Q80] 字符串截取
来源：http://gct.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nry.zdbjq.cn

[Q81] 字符串替换
来源：http://tzu.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kwz.dashuyun.cn

[Q82] 字符长度与字节长度
来源：http://hap.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fsx.vqdsnc.cn

[Q83] 大小写转换
来源：http://oty.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xca.gzhubu.top

[Q84] 去除首尾空格
来源：http://nvh.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://tgx.jinghuilouyu.cn

[Q85] 数值取整
来源：http://alu.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uyv.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://jmg.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cin.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://rjv.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uli.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://dud.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vhi.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tbo.smart0.xyz

[Q89] 判断表是否存在
来源：http://wsv.zhiwuduotai.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wxs.mhx1999.top

[Q90] 生成序号列
来源：http://mwn.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ndk.pengpengdd.cyou

================================================================================
来源：http://bpe.fktsv.cn

R. Bash 专题
来源：http://ats.shzxlz.cn

================================================================================
来源：http://hxf.epnwcf.com

[R01] shebang 与严格模式
来源：http://msw.havefunace.top

#!/usr/bin/env bash
来源：http://sno.jinghuilouyu.cn

set -euo pipefail
来源：http://qhh.ppjwa.cn

[R02] 变量赋值与使用
来源：http://xrt.guannengcc.top

name="Tom"; echo "$name"
来源：http://wfu.kuanghao11.cn

[R03] 只读变量
来源：http://vuo.tanke756.top

readonly PI=3.14
来源：http://uoy.svipenyu.cn

[R04] 位置参数
来源：http://pls.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://idi.zdqjudy.top

[R05] 参数默认值
来源：http://gnk.jyoumei.cn

name="${1:-default}"
来源：http://awc.bjfxy.top

[R06] 判断命令是否存在
来源：http://wfv.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mfq.xziqi.cn

[R07] if 判断文件
来源：http://qbt.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ieg.shanyushiyangtech.top

[R08] 数值比较
来源：http://fys.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lgh.uphjek.com

[R09] 字符串比较
来源：http://xmz.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oqz.yvedp.cn

[R10] 正则匹配
来源：http://ohu.fanxiaobao.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wyo.jinyuanbaomall.cn

[R11] case 多分支
来源：http://qmd.zhongyouzk.top

case "$1" in
来源：http://jgz.chenjidiqi.icu

start) echo "启动" ;;
来源：http://zpm.tanke756.top

stop)  echo "停止" ;;
来源：http://xll.tian-w.cn

*)     echo "未知命令" ;;
来源：http://vgj.cashguo.top

esac
来源：http://col.yueranfly.top

[R12] for 遍历文件
来源：http://sqd.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://tpv.fzhhl.top

[R13] for 计数循环
来源：http://uhi.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://pbq.fehbvm.com

[R14] C 风格 for
来源：http://jbl.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ril.bbcook.cn

[R15] while 逐行读文件
来源：http://ump.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://isc.sweek.top

[R16] until 等待条件
来源：http://cig.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://axx.shuidangran.top

[R17] 数组定义与取值
来源：http://jue.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vre.xuanzx.com

[R18] 遍历数组
来源：http://zpl.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dme.hywenlv.cn

[R19] 数组长度
来源：http://lcl.c1oappe.top

echo "${#arr[@]}"
来源：http://jot.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://tkl.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nza.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://wnm.yvedp.cn

echo "${#s}"
来源：http://ojs.0kj1m.cn

[R22] 截取子串
来源：http://vaa.pycfn.com

echo "${s:0:5}"
来源：http://jid.chenjidiqi.icu

[R23] 字符串替换
来源：http://lnx.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nvt.bjfxy.top

[R24] 大小写转换
来源：http://kos.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://qlu.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://got.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oic.ywan-chungtsiang.top

[R26] 命令替换
来源：http://zba.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://tsq.c1oappe.top

[R27] 算术展开
来源：http://ssw.xylfe.cn

echo $((1 + 2 * 3))
来源：http://rzk.sxryk.cn

[R28] 浮点运算
来源：http://lio.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://whk.nanxinkj.top

[R29] 定义函数
来源：http://swv.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yij.ydzc1.top

[R30] 函数返回状态码
来源：http://qhg.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://dbn.iojbl.cn

[R31] 局部变量
来源：http://ftp.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://iyp.yonumen.top

[R32] 参数个数校验
来源：http://yxa.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qpb.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://hkx.xingfuxueyuan.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jfo.nwbrower.top

[R34] 退出时清理
来源：http://dhq.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gnx.c1oappe.top

[R35] 后台执行并等待
来源：http://gfb.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tyd.ydzc1.top

[R36] 并发执行多个任务
来源：http://tyt.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xfr.cheryme.top

[R37] 把输出赋给变量
来源：http://bhk.zhixingplan.top

files=$(ls -1)
来源：http://cfr.sysykeji.top

[R38] 管道串联
来源：http://uzy.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://zvf.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://ecn.hysaishi.cn

cmd > out.log 2>&1
来源：http://nzh.nanxinkj.top

[R40] 追加写日志
来源：http://rkp.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://ghs.hysaishi.cn

[R41] 丢弃输出
来源：http://dtv.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://pqo.havefunace.top

[R42] 输入重定向
来源：http://saz.havefunace.top

wc -l < a.txt
来源：http://ikv.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://dyb.ydzc1.top

find . -name "*.log" -type f
来源：http://aip.bjfxy.top

[R44] 按修改时间查找
来源：http://huw.yj202588.top

find . -mtime -7 -type f
来源：http://zdx.hesvh.cn

[R45] 批量删除
来源：http://xua.cucudq.cn

find . -name "*.tmp" -delete
来源：http://nmc.gzhubu.top

[R46] 递归替换文件内容
来源：http://ygm.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://owv.epnwcf.com

[R47] sed 单行替换
来源：http://jjz.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ktw.yueranfly.top

[R48] awk 取指定列
来源：http://ebd.pengpengdd.cyou

awk '{print $1, $3}' a.txt
来源：http://ubg.tian-w.cn

[R49] awk 带条件
来源：http://pqc.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ywd.xuanzx.com

[R50] awk 求和
来源：http://vnz.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://bmm.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://axv.pengpengdd.cyou


<!-- 参考信息 -->