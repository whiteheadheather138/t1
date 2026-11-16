代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yny.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://lbz.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lps.sweek.top

[Q06] 删除列
来源：http://flj.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://xbr.xingfuxueyuan.xyz

[Q07] 删除表
来源：http://tot.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://dey.tanke756.top

[Q08] 创建普通索引
来源：http://boc.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://opb.nanxinkj.top

[Q09] 创建唯一索引
来源：http://cmi.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://awv.jinqigufen.top

[Q10] 插入单行
来源：http://bik.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tjy.bjfxy.top

[Q11] 一次插入多行
来源：http://aox.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xiy.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://zqd.hnqzz.top

INSERT INTO users (name) VALUES ('C');
来源：http://mdn.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gta.aizwys.cn

[Q13] 忽略重复插入
来源：http://cqf.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://abt.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://eoc.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cob.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iri.jqgufenzy.top

[Q15] 查询全部
来源：http://ypl.birdmap.top

SELECT * FROM users;
来源：http://ukr.zdbjq.cn

[Q16] 查询指定列
来源：http://uas.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://vgb.tanke756.top

[Q17] 条件查询
来源：http://lsw.bjfxy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gon.jyoumei.cn

[Q18] 模糊匹配
来源：http://lqj.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wfq.hcnkem.com

[Q19] 范围查询
来源：http://eja.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xnp.zhoulong.xyz

[Q20] IN 列表
来源：http://slp.dianchejie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xoe.hfpthk.cn

[Q21] 空值判断
来源：http://jlo.birdmap.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aiz.fktsv.cn

[Q22] 排序
来源：http://gjr.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rya.fanxiaobao.xyz

[Q23] 分页
来源：http://qsk.fengsongda.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rgc.yonumen.top

[Q24] 去重
来源：http://uch.aibaodan.cn

SELECT DISTINCT city FROM users;
来源：http://nqb.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://fkd.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iyd.birdmap.top

[Q26] 计数
来源：http://jau.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://lxc.daria6918.cn

[Q27] 条件计数
来源：http://vuk.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://guh.jqgufenzy.top

[Q28] 求和与平均
来源：http://xsq.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mto.cheryme.top

[Q29] 最大最小值
来源：http://xrp.yangfankeji.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://apk.zdbjq.cn

[Q30] 分组统计
来源：http://qfg.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aae.gotoacloud.top

[Q31] 分组后过滤
来源：http://cpn.tian-w.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ppz.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://kal.nanxinkj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sjl.tian-w.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hol.quarkkingdee.top

[Q33] 多列分组
来源：http://hiv.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qii.sweek.top

[Q34] 每组取第一条
来源：http://ptx.ywan-chungtsiang.top

SELECT * FROM (
来源：http://qzl.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kye.chenlongwang.top

) t WHERE rn = 1;
来源：http://sdp.xuetiantiany.cn

[Q35] 内连接
来源：http://avm.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qpm.52xcode.cn

[Q36] 左连接
来源：http://mvr.havefunace.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kox.bjfxy.top

[Q37] 右连接
来源：http://oft.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://awz.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://nrv.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gpi.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://nbx.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://joj.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://czt.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jpr.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gol.vehdjk.com

[Q41] 多表连接
来源：http://kiy.sweek.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pjw.chenjidiqi.icu

JOIN users u ON u.id = o.user_id
来源：http://pzy.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://yax.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://rcy.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://hmr.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hyn.hesvh.cn

[Q43] 标量子查询
来源：http://zaf.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ovo.jiagoushi.top

[Q44] IN 子查询
来源：http://aum.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zbt.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://dxh.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://omq.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://qyz.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://map.gzhubu.top

[Q47] 与平均值比较
来源：http://bzp.jinqigfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rca.316326.xyz

[Q48] CTE 公用表表达式
来源：http://pem.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://set.daria6918.cn

SELECT * FROM t WHERE c > 5;
来源：http://oxx.havefunace.top

[Q49] 更新单行
来源：http://vup.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vgn.9152youxi.cn

[Q50] 批量更新
来源：http://odj.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zyd.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://huz.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ofk.hysaishi.cn

[Q52] 删除指定行
来源：http://ovy.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://flj.fehbvm.com

[Q53] 按条件删除
来源：http://ltz.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jjc.shanyushiyangtech.top

[Q54] 清空表
来源：http://pdg.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://dfe.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://pgq.shangyingyoupin.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iak.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://ytw.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dun.wangdashe.top

[Q57] 行号
来源：http://mta.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wjk.tian-w.cn

[Q58] 累计求和
来源：http://nvd.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ebc.redwolf501.top

[Q59] 分组内累计
来源：http://yux.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uci.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://bhy.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lha.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nka.cheryme.top

[Q61] 移动平均
来源：http://naw.zhengqikj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://trg.cucudq.cn

[Q62] 分组占比
来源：http://sjr.zhoulong.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cas.redwolf501.top

[Q63] 开启事务
来源：http://kgw.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vly.ehwqpu.com

[Q64] 提交事务
来源：http://idv.zhongyouzk.top

COMMIT;
来源：http://czf.316326.xyz

[Q65] 回滚事务
来源：http://nci.jinqigfzy.top

ROLLBACK;
来源：http://mpq.jianghu66.top

[Q66] 行锁查询
来源：http://hcs.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://btf.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://zts.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://klj.yonumen.top

[Q68] 保存点
来源：http://jff.xinyue.icu

SAVEPOINT sp1;
来源：http://kwx.yuxming.cn

ROLLBACK TO sp1;
来源：http://kqw.yj20258888.top

[Q69] 查看执行计划
来源：http://pxy.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rru.birdmap.top

[Q70] 更新统计信息
来源：http://abg.dianchejie.cn

ANALYZE TABLE users;
来源：http://jjc.yuxming.cn

[Q71] 查看建表语句
来源：http://uob.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://psr.haohaochexian.top

[Q72] 查看索引
来源：http://zkj.snrcjt.cn

SHOW INDEX FROM users;
来源：http://rex.hongshengwenyu.top

[Q73] 查看表状态
来源：http://oir.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nxs.ydzc1.top

[Q74] 强制使用索引
来源：http://jin.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xuj.dianchejie.cn

[Q75] 日期格式化
来源：http://deg.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rpi.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dlm.zhengqikj.top

[Q76] 按天统计
来源：http://xdy.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xyh.aibaodan.cn

[Q77] 时间加减
来源：http://ewm.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ygk.hysaishi.cn

[Q78] 当前时间
来源：http://baa.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mpl.gotoacloud.top

[Q79] 字符串拼接
来源：http://vdk.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wzo.hammf.cn

[Q80] 字符串截取
来源：http://lqn.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cjw.wangshuangyany.cn

[Q81] 字符串替换
来源：http://qvf.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yyv.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://xmo.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://boy.andypj.xyz

[Q83] 大小写转换
来源：http://flr.uphjek.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qao.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://hoc.uphjek.com

SELECT TRIM(name) FROM users;
来源：http://oom.yuanzhike.top

[Q85] 数值取整
来源：http://ayp.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bcb.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://syv.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dbf.yfazqb.com

[Q87] JSON 字段做条件
来源：http://msh.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hjy.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://fbq.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lfm.tianlin.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bee.fktsv.cn

[Q89] 判断表是否存在
来源：http://ydr.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uqm.jianghu66.top

[Q90] 生成序号列
来源：http://wco.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kdg.jyoumei.cn

================================================================================
来源：http://cmx.havefunace.top

R. Bash 专题
来源：http://ugi.tarul.cn

================================================================================
来源：http://ukp.sweek.top

[R01] shebang 与严格模式
来源：http://ncy.yanxiufei.cn

#!/usr/bin/env bash
来源：http://vms.wangdashe.top

set -euo pipefail
来源：http://lkw.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://dsb.tarul.cn

name="Tom"; echo "$name"
来源：http://jxq.tanke756.top

[R03] 只读变量
来源：http://rmn.jiagoushi.top

readonly PI=3.14
来源：http://zec.zhiwuduotai.top

[R04] 位置参数
来源：http://jxm.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lyr.nanxuanxn.top

[R05] 参数默认值
来源：http://ndx.iojbl.cn

name="${1:-default}"
来源：http://wrh.wangdashe.top

[R06] 判断命令是否存在
来源：http://amw.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iuf.shuidangran.top

[R07] if 判断文件
来源：http://kag.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mkd.jinyuanbaomall.cn

[R08] 数值比较
来源：http://tpg.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hiz.sufxvd.cn

[R09] 字符串比较
来源：http://hgb.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ijv.birdmap.top

[R10] 正则匹配
来源：http://kyb.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jrn.xylfe.cn

[R11] case 多分支
来源：http://mij.c1oappe.top

case "$1" in
来源：http://wds.hesvh.cn

start) echo "启动" ;;
来源：http://hgu.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://ubu.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://rmd.birdmap.top

esac
来源：http://eyl.zhongyouzk.top

[R12] for 遍历文件
来源：http://exj.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://ggq.wangdashe.top

[R13] for 计数循环
来源：http://fwn.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://vzu.jianghu66.top

[R14] C 风格 for
来源：http://ect.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wci.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://aax.snrcjt.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fpb.cheryme.top

[R16] until 等待条件
来源：http://otn.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hoq.yvedp.cn

[R17] 数组定义与取值
来源：http://kwz.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://cbc.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://ckj.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hdd.fzhhl.top

[R19] 数组长度
来源：http://nvu.9152youxi.cn

echo "${#arr[@]}"
来源：http://ixa.birdmap.top

[R20] 关联数组（字典）
来源：http://gnu.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jko.daria6918.cn

[R21] 字符串长度
来源：http://mhc.shangyingyoupin.top

echo "${#s}"
来源：http://cgg.jqgfzy.top

[R22] 截取子串
来源：http://sdi.guannengcc.top

echo "${s:0:5}"
来源：http://jjt.chenjidiqi.icu

[R23] 字符串替换
来源：http://ehv.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pzk.ydjk.org.cn

[R24] 大小写转换
来源：http://vty.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://pvg.jlsjyb.cn

[R25] 去后缀 / 去前缀
来源：http://hqv.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://tjy.xuanzx.com

[R26] 命令替换
来源：http://diq.pycfn.com

now=$(date +%F); echo "$now"
来源：http://juq.ybcxt.top

[R27] 算术展开
来源：http://xet.daria6918.cn

echo $((1 + 2 * 3))
来源：http://hpr.fzhhl.top

[R28] 浮点运算
来源：http://los.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://zzw.chenjidiqi.icu

[R29] 定义函数
来源：http://vzw.zdqjudy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ugz.guowangkeji.top

[R30] 函数返回状态码
来源：http://hrl.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://ain.fengsongda.top

[R31] 局部变量
来源：http://tll.yj20258.top

f() { local x=1; echo "$x"; }
来源：http://fnd.tianlin.xyz

[R32] 参数个数校验
来源：http://soz.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cfp.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://goy.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ioy.quarkkingdee.top

[R34] 退出时清理
来源：http://cjl.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://tuc.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://diz.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ajk.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://ntm.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pnb.yvedp.cn

[R37] 把输出赋给变量
来源：http://kso.bbcook.cn

files=$(ls -1)
来源：http://cjn.tian-w.cn

[R38] 管道串联
来源：http://slf.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://fli.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://bdq.ydjk.org.cn

cmd > out.log 2>&1
来源：http://ssq.kuanghao11.cn

[R40] 追加写日志
来源：http://yey.c1oappe.top

echo "log" >> out.log
来源：http://nyg.shuidangran.top

[R41] 丢弃输出
来源：http://ffg.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://yzm.tian-w.cn

[R42] 输入重定向
来源：http://hly.wangdashe.top

wc -l < a.txt
来源：http://mbj.yuxming.cn

[R43] 按名字查找文件
来源：http://vwn.hnqzz.top

find . -name "*.log" -type f
来源：http://uaq.ctjpmb.com

[R44] 按修改时间查找
来源：http://znj.fktsv.cn

find . -mtime -7 -type f
来源：http://lfd.zhijiandao.cn

[R45] 批量删除
来源：http://pgv.sweek.top

find . -name "*.tmp" -delete
来源：http://pds.hammf.cn

[R46] 递归替换文件内容
来源：http://rus.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hlk.fktsv.cn

[R47] sed 单行替换
来源：http://yiz.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://vhj.feifeiyinyue.top

[R48] awk 取指定列
来源：http://nlk.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://hoe.xuetiantiany.cn

[R49] awk 带条件
来源：http://bfa.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lth.ydzc1.top

[R50] awk 求和
来源：http://plk.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dem.zdqjudy.top

[R51] 排序去重取前几
来源：http://yez.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hyr.hnxiangtu.top

[R52] 统计行数
来源：http://xhw.shangyingyoupin.top

wc -l a.txt
来源：http://ank.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://soj.52xcode.cn


<!-- 参考信息 -->