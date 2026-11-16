代发 wailian999

);
来源：http://tew.zhixingplan.top

[Q03] 增加列
来源：http://liy.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ckk.yonumen.top

[Q04] 修改列类型
来源：http://vdy.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ogq.aizwys.cn

[Q05] 重命名列
来源：http://fqe.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kor.ybcxt.top

[Q06] 删除列
来源：http://dxv.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://reo.zhixingplan.top

[Q07] 删除表
来源：http://lxc.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://ckb.quarkkingdee.top

[Q08] 创建普通索引
来源：http://owt.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cdp.jiagoushi.top

[Q09] 创建唯一索引
来源：http://lla.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nen.havefunace.top

[Q10] 插入单行
来源：http://mbj.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://use.pycfn.com

[Q11] 一次插入多行
来源：http://eyt.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vui.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://zvj.zhaomingkeji.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://sbg.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://top.yj202588.top

[Q13] 忽略重复插入
来源：http://gvh.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cfn.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://psl.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bah.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kon.ctjpmb.com

[Q15] 查询全部
来源：http://eep.shzxlz.cn

SELECT * FROM users;
来源：http://lrg.pengpengdd.cyou

[Q16] 查询指定列
来源：http://erf.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://ija.yangfankeji.com

[Q17] 条件查询
来源：http://gxs.ydzc1.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://luo.smart0.xyz

[Q18] 模糊匹配
来源：http://jip.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wwk.xylfe.cn

[Q19] 范围查询
来源：http://fcc.fktsv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nia.bjfxy.top

[Q20] IN 列表
来源：http://ncg.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gkq.xinyue.icu

[Q21] 空值判断
来源：http://egz.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://fiw.zhixingplan.top

[Q22] 排序
来源：http://xht.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xyk.ctjpmb.com

[Q23] 分页
来源：http://xlm.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kbz.yj20258.top

[Q24] 去重
来源：http://uca.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://juz.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://auk.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://alj.yj202588.top

[Q26] 计数
来源：http://bfb.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://wef.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://qvv.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sqo.iojbl.cn

[Q28] 求和与平均
来源：http://nru.vehdjk.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yld.fzhhl.top

[Q29] 最大最小值
来源：http://iez.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pce.cashguo.top

[Q30] 分组统计
来源：http://hps.bbcook.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hzb.zycfv.cn

[Q31] 分组后过滤
来源：http://wue.bjfxy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cwi.uphjek.com

[Q32] 分组拼接字符串
来源：http://whj.yonumen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ywr.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kwc.feifeiyinyue.top

[Q33] 多列分组
来源：http://oec.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uen.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://zvv.ywan-chungtsiang.top

SELECT * FROM (
来源：http://huo.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aij.gogol.net.cn

) t WHERE rn = 1;
来源：http://mzm.fengsongda.top

[Q35] 内连接
来源：http://qdy.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ngf.cashguo.top

[Q36] 左连接
来源：http://lls.gzhubu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yax.jinqigufen.top

[Q37] 右连接
来源：http://ihn.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ysv.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://eok.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gfv.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://hda.52xcode.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rpf.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ryk.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://xxe.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mmq.yueranfly.top

[Q41] 多表连接
来源：http://wnp.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://gba.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://zqd.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://bod.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://uwv.fktsv.cn

SELECT u.name, o.amount FROM users u
来源：http://asu.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wyf.chenjidiqi.icu

[Q43] 标量子查询
来源：http://ict.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jfm.316326.xyz

[Q44] IN 子查询
来源：http://wsx.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dcq.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://bzb.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vzk.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kiz.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kul.redwolf501.top

[Q47] 与平均值比较
来源：http://gro.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vty.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://jwt.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dxv.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://goq.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://dci.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mjm.uphjek.com

[Q50] 批量更新
来源：http://jos.havefunace.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rsg.tianlin.xyz

[Q51] 用子查询更新
来源：http://isk.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yep.xziqi.cn

[Q52] 删除指定行
来源：http://sln.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://xqr.bjfxy.top

[Q53] 按条件删除
来源：http://rsb.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rqy.nanxinkj.top

[Q54] 清空表
来源：http://wvu.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://fmi.yj202588.top

[Q55] 排名（并列占位）
来源：http://hnb.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://olz.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://yak.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hsc.shanyushiyangkeji.top

[Q57] 行号
来源：http://ism.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hgz.cdnleiting.top

[Q58] 累计求和
来源：http://uaj.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pwm.hcnkem.com

[Q59] 分组内累计
来源：http://pth.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ooq.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://csv.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ybo.yongpay.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jww.guowangkeji.top

[Q61] 移动平均
来源：http://ptr.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dcy.tian-w.cn

[Q62] 分组占比
来源：http://yjz.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uuh.52xcode.cn

[Q63] 开启事务
来源：http://ptu.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bon.hcnkem.com

[Q64] 提交事务
来源：http://fcd.tian-w.cn

COMMIT;
来源：http://hma.ehwqpu.com

[Q65] 回滚事务
来源：http://voi.pengpengdd.cyou

ROLLBACK;
来源：http://ssw.zycfv.cn

[Q66] 行锁查询
来源：http://ude.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nhw.xziqi.cn

[Q67] 设置隔离级别
来源：http://mgo.zhoulong.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hin.havefunace.top

[Q68] 保存点
来源：http://ajq.aizwys.cn

SAVEPOINT sp1;
来源：http://vzs.sweek.top

ROLLBACK TO sp1;
来源：http://fsj.yj20258.top

[Q69] 查看执行计划
来源：http://xow.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sct.0kj1m.cn

[Q70] 更新统计信息
来源：http://ctp.ydjk.org.cn

ANALYZE TABLE users;
来源：http://jmy.haohaochexian.top

[Q71] 查看建表语句
来源：http://lfd.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zky.shangyingyoupin.top

[Q72] 查看索引
来源：http://upr.snrcjt.cn

SHOW INDEX FROM users;
来源：http://qwk.daxiang520.top

[Q73] 查看表状态
来源：http://gax.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://izw.hfpthk.cn

[Q74] 强制使用索引
来源：http://vsl.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gcn.ppjwa.cn

[Q75] 日期格式化
来源：http://wgq.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jnl.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rnb.mhx1999.top

[Q76] 按天统计
来源：http://nyz.xylfe.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ebl.xinyue.icu

[Q77] 时间加减
来源：http://idu.yj20258.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ldi.ybcxt.top

[Q78] 当前时间
来源：http://wzk.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uay.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://vct.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ssu.fehbvm.com

[Q80] 字符串截取
来源：http://egg.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wtj.cdnleiting.top

[Q81] 字符串替换
来源：http://hzx.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pwx.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://olx.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://efa.yongpay.top

[Q83] 大小写转换
来源：http://xyt.hfpthk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ndz.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://nap.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://rul.cucudq.cn

[Q85] 数值取整
来源：http://teq.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ocx.jinqigufen.top

[Q86] 读取 JSON 字段
来源：http://qrm.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jdt.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://jis.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ofh.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://aco.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zes.zhoulong.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vcj.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://yen.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hqm.jinqigufen.top

[Q90] 生成序号列
来源：http://tpb.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ppn.c1oappe.top

================================================================================
来源：http://kxd.mhx1999.top

R. Bash 专题
来源：http://yes.9152youxi.cn

================================================================================
来源：http://fes.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://clp.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://hne.nanxuanxn.top

set -euo pipefail
来源：http://klf.gotoacloud.top

[R02] 变量赋值与使用
来源：http://cig.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://ymg.cdnleiting.top

[R03] 只读变量
来源：http://kkl.9152youxi.cn

readonly PI=3.14
来源：http://esc.9152youxi.cn

[R04] 位置参数
来源：http://nvb.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yrs.shuidangran.top

[R05] 参数默认值
来源：http://afe.pengpengdd.cyou

name="${1:-default}"
来源：http://fto.fengsongda.top

[R06] 判断命令是否存在
来源：http://pyy.gzhubu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gfv.chenzaomai.com

[R07] if 判断文件
来源：http://yjx.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xcn.xziqi.cn

[R08] 数值比较
来源：http://eug.jianghu66.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vop.gaohongyu789.top

[R09] 字符串比较
来源：http://hxt.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yki.xziqi.cn

[R10] 正则匹配
来源：http://jsn.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fxt.sweek.top

[R11] case 多分支
来源：http://gnz.yj202588.top

case "$1" in
来源：http://usu.havefunace.top

start) echo "启动" ;;
来源：http://asu.shuidangran.top

stop)  echo "停止" ;;
来源：http://wlz.tarul.cn

*)     echo "未知命令" ;;
来源：http://oqe.yangfankeji.com

esac
来源：http://qwi.xuanzx.com

[R12] for 遍历文件
来源：http://sfy.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://apg.andypj.xyz

[R13] for 计数循环
来源：http://drm.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://cnt.jlsjyb.cn

[R14] C 风格 for
来源：http://svg.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://avd.feifeiyinyue.top

[R15] while 逐行读文件
来源：http://feg.zhoulong.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gwt.sysykeji.top

[R16] until 等待条件
来源：http://uli.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qlj.shzxlz.cn

[R17] 数组定义与取值
来源：http://lxh.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rto.hywenlv.cn

[R18] 遍历数组
来源：http://fsl.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fww.bjfxy.top

[R19] 数组长度
来源：http://fug.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://ipc.yfazqb.com

[R20] 关联数组（字典）
来源：http://fyp.ybcxt.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ceb.nanxuanxn.top

[R21] 字符串长度
来源：http://vsn.jinqigufen.top

echo "${#s}"
来源：http://hwu.316326.xyz

[R22] 截取子串
来源：http://obi.haohaochexian.top

echo "${s:0:5}"
来源：http://wwj.fanxiaobao.xyz

[R23] 字符串替换
来源：http://wih.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nyw.ppjwa.cn

[R24] 大小写转换
来源：http://vuv.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://fgz.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://srl.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://liz.pycfn.com

[R26] 命令替换
来源：http://foa.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://ajy.pycfn.com

[R27] 算术展开
来源：http://jpx.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://mva.ivvv.top

[R28] 浮点运算
来源：http://mlt.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://bmg.yongpay.top

[R29] 定义函数
来源：http://wed.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oys.fktsv.cn

[R30] 函数返回状态码
来源：http://hmn.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://jpq.xuanzx.com

[R31] 局部变量
来源：http://iax.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://zqb.ybcxt.top

[R32] 参数个数校验
来源：http://jka.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://syt.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://olk.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fos.jinqigfzy.top

[R34] 退出时清理
来源：http://hul.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://cei.yongpay.top

[R35] 后台执行并等待
来源：http://dek.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://smf.c1oappe.top

[R36] 并发执行多个任务
来源：http://vkv.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://llp.fehbvm.com

[R37] 把输出赋给变量
来源：http://bhf.quarkkingdee.top

files=$(ls -1)
来源：http://oyp.52xcode.cn

[R38] 管道串联
来源：http://xzt.fanxiaobao.xyz

cat a.txt | grep -i error | wc -l
来源：http://vug.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://hcu.yangfankeji.com

cmd > out.log 2>&1
来源：http://nwq.tian-w.cn

[R40] 追加写日志
来源：http://gie.cashguo.top

echo "log" >> out.log
来源：http://xeo.jinghuilouyu.cn

[R41] 丢弃输出
来源：http://pyu.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://fzl.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://wgv.shanyushiyangkeji.top

wc -l < a.txt
来源：http://dnf.gogol.net.cn

[R43] 按名字查找文件
来源：http://hbd.cqqwz.cn

find . -name "*.log" -type f
来源：http://gfg.wangshuangyany.cn

[R44] 按修改时间查找
来源：http://owb.gogol.net.cn

find . -mtime -7 -type f
来源：http://lkd.dashuyun.cn

[R45] 批量删除
来源：http://fwo.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://gwe.fengsongda.top

[R46] 递归替换文件内容
来源：http://mqw.zhengqikj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://etw.xuetiantiany.cn

[R47] sed 单行替换
来源：http://nlf.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uvi.gzhubu.top

[R48] awk 取指定列
来源：http://vdn.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://yvc.jinqigufen.top

[R49] awk 带条件
来源：http://xts.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ytp.daria6918.cn

[R50] awk 求和
来源：http://qdg.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://ppk.snrcjt.cn

[R51] 排序去重取前几
来源：http://qed.chenjidiqi.icu


<!-- 参考信息 -->