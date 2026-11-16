代发 wailian999

);
来源：http://ypq.sxryk.cn

[Q03] 增加列
来源：http://sfj.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sob.yonumen.top

[Q04] 修改列类型
来源：http://epl.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rxt.zhoulong.xyz

[Q05] 重命名列
来源：http://jaz.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ciu.ctjpmb.com

[Q06] 删除列
来源：http://hfz.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sfb.ywan-chungtsiang.top

[Q07] 删除表
来源：http://yal.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://cmb.xylfe.cn

[Q08] 创建普通索引
来源：http://ffg.pycfn.com

CREATE INDEX idx_users_email ON users(email);
来源：http://loe.birdmap.top

[Q09] 创建唯一索引
来源：http://frd.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ppm.xziqi.cn

[Q10] 插入单行
来源：http://xkd.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cag.hcnkem.com

[Q11] 一次插入多行
来源：http://bfn.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ftq.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://pkl.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://gso.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lza.yuxming.cn

[Q13] 忽略重复插入
来源：http://qre.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xoa.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://owr.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hxp.xuetiantiany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jwf.tian-w.cn

[Q15] 查询全部
来源：http://nlx.316326.xyz

SELECT * FROM users;
来源：http://adj.cashguo.top

[Q16] 查询指定列
来源：http://gtg.yongpay.top

SELECT id, name FROM users;
来源：http://fmc.dianchejie.cn

[Q17] 条件查询
来源：http://hxd.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://das.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://ifo.zhixingplan.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cwn.shanyushiyangtech.top

[Q19] 范围查询
来源：http://xyq.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fbo.sweek.top

[Q20] IN 列表
来源：http://vma.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zha.c1oappe.top

[Q21] 空值判断
来源：http://pgv.yangfankeji.com

SELECT * FROM users WHERE email IS NULL;
来源：http://obw.nanxuanxn.top

[Q22] 排序
来源：http://bag.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nmj.yvedp.cn

[Q23] 分页
来源：http://zmu.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iui.uphjek.com

[Q24] 去重
来源：http://fuk.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://xvl.hammf.cn

[Q25] 只取前 N 条
来源：http://uof.c1oappe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zgw.jinghuilouyu.cn

[Q26] 计数
来源：http://lax.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://lue.ctjpmb.com

[Q27] 条件计数
来源：http://sqa.jinghuilouyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rgz.jinyuanbaomall.cn

[Q28] 求和与平均
来源：http://ogx.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://trm.meibo888.top

[Q29] 最大最小值
来源：http://zwj.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xyk.shzxlz.cn

[Q30] 分组统计
来源：http://oib.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vka.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://gdf.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://htb.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://hnl.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uoe.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wua.yangfankeji.com

[Q33] 多列分组
来源：http://ykr.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://knw.52xcode.cn

[Q34] 每组取第一条
来源：http://fnh.hysaishi.cn

SELECT * FROM (
来源：http://mhk.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://odt.gzhubu.top

) t WHERE rn = 1;
来源：http://qjm.gotoacloud.top

[Q35] 内连接
来源：http://njt.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ffz.haohaochexian.top

[Q36] 左连接
来源：http://bup.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ycv.aizwys.cn

[Q37] 右连接
来源：http://nqd.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fht.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lvy.jlsjyb.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bbs.uphjek.com

[Q39] 自连接（查上下级）
来源：http://uwq.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ltg.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hgd.svipenyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pzl.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uqp.ppjwa.cn

[Q41] 多表连接
来源：http://xmm.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mrw.dianchejie.cn

JOIN users u ON u.id = o.user_id
来源：http://ufw.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://aji.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://nmg.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://kdi.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nid.yonumen.top

[Q43] 标量子查询
来源：http://mbe.yvedp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hxo.hesvh.cn

[Q44] IN 子查询
来源：http://tef.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hco.hnqzz.top

[Q45] EXISTS 判断存在
来源：http://nud.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://daj.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gsz.uphjek.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kdx.yuanzhike.top

[Q47] 与平均值比较
来源：http://xjb.yangfankeji.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ldo.jinghuilouyu.cn

[Q48] CTE 公用表表达式
来源：http://drf.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xra.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://snl.ehwqpu.com

[Q49] 更新单行
来源：http://mvl.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pyz.316326.xyz

[Q50] 批量更新
来源：http://ykx.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cex.havefunace.top

[Q51] 用子查询更新
来源：http://dhf.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fnq.ctjpmb.com

[Q52] 删除指定行
来源：http://zqt.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://two.meibo888.top

[Q53] 按条件删除
来源：http://jpi.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wce.ywan-chungtsiang.top

[Q54] 清空表
来源：http://sox.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://gzq.xziqi.cn

[Q55] 排名（并列占位）
来源：http://ous.tian-w.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pzf.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://bje.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://skj.ydjk.org.cn

[Q57] 行号
来源：http://zdd.jqgfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://syy.chenzaomai.com

[Q58] 累计求和
来源：http://irc.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ahl.bbcook.cn

[Q59] 分组内累计
来源：http://pcd.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wqp.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://iqs.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iyb.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ecs.havefunace.top

[Q61] 移动平均
来源：http://jry.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://trt.sjlbkw.cn

[Q62] 分组占比
来源：http://zzr.ivvv.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sxl.hfpthk.cn

[Q63] 开启事务
来源：http://gyu.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dbb.chenzaomai.com

[Q64] 提交事务
来源：http://kah.jqgfzy.top

COMMIT;
来源：http://wym.zdbjq.cn

[Q65] 回滚事务
来源：http://wvs.yanxiufei.cn

ROLLBACK;
来源：http://ruv.birdmap.top

[Q66] 行锁查询
来源：http://agk.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tfa.zdqjudy.top

[Q67] 设置隔离级别
来源：http://ces.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sdj.sysykeji.top

[Q68] 保存点
来源：http://xxq.aibaodan.cn

SAVEPOINT sp1;
来源：http://odx.yuxming.cn

ROLLBACK TO sp1;
来源：http://gbq.yvedp.cn

[Q69] 查看执行计划
来源：http://txh.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://udb.tarul.cn

[Q70] 更新统计信息
来源：http://vpi.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://zle.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://cip.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zqj.shangyingyoupin.top

[Q72] 查看索引
来源：http://ska.cdnleiting.top

SHOW INDEX FROM users;
来源：http://bbd.xinyue.icu

[Q73] 查看表状态
来源：http://ahy.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wea.hesvh.cn

[Q74] 强制使用索引
来源：http://pih.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bxk.pycfn.com

[Q75] 日期格式化
来源：http://for.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gvd.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sta.sysykeji.top

[Q76] 按天统计
来源：http://rno.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ouf.redwolf501.top

[Q77] 时间加减
来源：http://ibc.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://svp.pengpengdd.cyou

[Q78] 当前时间
来源：http://qap.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ask.epnwcf.com

[Q79] 字符串拼接
来源：http://ezg.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://guy.316326.xyz

[Q80] 字符串截取
来源：http://ipq.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qwi.dashuyun.cn

[Q81] 字符串替换
来源：http://fte.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ptv.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://iar.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hpd.feifeiyinyue.top

[Q83] 大小写转换
来源：http://bzu.cqqwz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yyu.c1oappe.top

[Q84] 去除首尾空格
来源：http://fdc.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://tpm.dashuyun.cn

[Q85] 数值取整
来源：http://bjy.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ldb.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://tai.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zst.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://iwc.zhongyouzk.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eic.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://pem.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qmc.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ves.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://dls.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bqx.ehwqpu.com

[Q90] 生成序号列
来源：http://hpx.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zee.xuetiantiany.cn

================================================================================
来源：http://okt.sysykeji.top

R. Bash 专题
来源：http://xrq.gogol.net.cn

================================================================================
来源：http://edr.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://vfs.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://pmz.xylfe.cn

set -euo pipefail
来源：http://hur.jinqigufen.top

[R02] 变量赋值与使用
来源：http://mnj.cdnleiting.top

name="Tom"; echo "$name"
来源：http://ibv.tianlin.xyz

[R03] 只读变量
来源：http://uhk.ivvv.top

readonly PI=3.14
来源：http://zgo.ehwqpu.com

[R04] 位置参数
来源：http://tuw.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ztd.zycfv.cn

[R05] 参数默认值
来源：http://ffs.xinyue.icu

name="${1:-default}"
来源：http://scp.hnxiangtu.top

[R06] 判断命令是否存在
来源：http://gqq.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iii.guannengcc.top

[R07] if 判断文件
来源：http://vuy.zhengqikj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pgh.vqdsnc.cn

[R08] 数值比较
来源：http://ihs.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jtm.feifeiyinyue.top

[R09] 字符串比较
来源：http://kxj.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gcn.ehwqpu.com

[R10] 正则匹配
来源：http://oux.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wwz.jinghuilouyu.cn

[R11] case 多分支
来源：http://vzg.hywenlv.cn

case "$1" in
来源：http://qxj.bjfxy.top

start) echo "启动" ;;
来源：http://lcq.havefunace.top

stop)  echo "停止" ;;
来源：http://kfs.tanke756.top

*)     echo "未知命令" ;;
来源：http://erq.hfpthk.cn

esac
来源：http://cpu.hammf.cn

[R12] for 遍历文件
来源：http://tib.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://hmg.fktsv.cn

[R13] for 计数循环
来源：http://qhk.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://wgq.aizwys.cn

[R14] C 风格 for
来源：http://ntu.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pzs.zhijiandao.cn

[R15] while 逐行读文件
来源：http://ifo.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hxr.cucudq.cn

[R16] until 等待条件
来源：http://gzg.smart0.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nov.zhoulong.xyz

[R17] 数组定义与取值
来源：http://nwg.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xyu.ydzc1.top

[R18] 遍历数组
来源：http://iqc.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ysg.52xcode.cn

[R19] 数组长度
来源：http://ghm.zdqjudy.top

echo "${#arr[@]}"
来源：http://xhd.uphjek.com

[R20] 关联数组（字典）
来源：http://nlv.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fwc.birdmap.top

[R21] 字符串长度
来源：http://ezm.wangdashe.top

echo "${#s}"
来源：http://jcy.zycfv.cn

[R22] 截取子串
来源：http://rvx.zhoulong.xyz

echo "${s:0:5}"
来源：http://tqn.nanxinkj.top

[R23] 字符串替换
来源：http://tkq.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ofy.daria6918.cn

[R24] 大小写转换
来源：http://xuu.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qut.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://hil.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mmu.gaohongyu789.top

[R26] 命令替换
来源：http://hgh.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://iif.mhx1999.top

[R27] 算术展开
来源：http://fgy.52xcode.cn

echo $((1 + 2 * 3))
来源：http://jes.yj20258888.top

[R28] 浮点运算
来源：http://abd.zhiwuduotai.top

echo "scale=2; 10/3" | bc
来源：http://ovr.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://lvk.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xon.yangfankeji.com

[R30] 函数返回状态码
来源：http://vfx.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://yzo.shzxlz.cn

[R31] 局部变量
来源：http://ggz.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://rji.cheryme.top

[R32] 参数个数校验
来源：http://ojx.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hlk.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://ufv.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://htc.yonumen.top

[R34] 退出时清理
来源：http://wrp.cheryme.top

trap 'rm -f "$tmp"' EXIT
来源：http://xya.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://txz.gotoacloud.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dbf.havefunace.top

[R36] 并发执行多个任务
来源：http://rea.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dhp.tian-w.cn

[R37] 把输出赋给变量
来源：http://ewf.xylfe.cn

files=$(ls -1)
来源：http://nok.fzhhl.top

[R38] 管道串联
来源：http://krs.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://snp.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://tux.jqgfzy.top

cmd > out.log 2>&1
来源：http://oid.yangfankeji.com

[R40] 追加写日志
来源：http://iki.316326.xyz

echo "log" >> out.log
来源：http://bsg.shuidangran.top

[R41] 丢弃输出
来源：http://blo.meibo888.top

cmd >/dev/null 2>&1
来源：http://mzv.yuxming.cn

[R42] 输入重定向
来源：http://yjd.xingfuxueyuan.xyz

wc -l < a.txt
来源：http://lki.316326.xyz

[R43] 按名字查找文件
来源：http://cvb.chenlongwang.top

find . -name "*.log" -type f
来源：http://gwe.zhoulong.xyz

[R44] 按修改时间查找
来源：http://trr.ybcxt.top

find . -mtime -7 -type f
来源：http://pkl.316326.xyz

[R45] 批量删除
来源：http://rqv.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://fty.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://mku.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ndk.yj20258.top

[R47] sed 单行替换
来源：http://whi.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lyz.fzhhl.top

[R48] awk 取指定列
来源：http://ity.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://dbv.chenzaomai.com

[R49] awk 带条件
来源：http://gqb.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pzg.jiagoushi.top

[R50] awk 求和
来源：http://jgs.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://amj.zhoulong.xyz

[R51] 排序去重取前几
来源：http://izl.meibo888.top


<!-- 参考信息 -->