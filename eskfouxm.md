代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uwa.xylfe.cn

user_id INT NOT NULL,
来源：http://mxi.jianghu66.top

amount DECIMAL(10, 2),
来源：http://nmf.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ljx.fanxiaobao.xyz

);
来源：http://dwc.c1oappe.top

[Q03] 增加列
来源：http://iil.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xwm.hongshengwenyu.top

[Q04] 修改列类型
来源：http://kks.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nxm.0kj1m.cn

[Q05] 重命名列
来源：http://chj.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sne.ivvv.top

[Q06] 删除列
来源：http://dlt.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://myk.fehbvm.com

[Q07] 删除表
来源：http://njl.c1oappe.top

DROP TABLE IF EXISTS orders;
来源：http://zvo.smart0.xyz

[Q08] 创建普通索引
来源：http://otd.zycfv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oim.chenzaomai.com

[Q09] 创建唯一索引
来源：http://rsv.xuanzx.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://plc.vehdjk.com

[Q10] 插入单行
来源：http://gca.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://twk.tarul.cn

[Q11] 一次插入多行
来源：http://yjc.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://okv.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://wyw.zhixingplan.top

INSERT INTO users (name) VALUES ('C');
来源：http://xyc.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vmr.sxryk.cn

[Q13] 忽略重复插入
来源：http://ewp.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://naj.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://umi.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zvg.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bkz.cdnleiting.top

[Q15] 查询全部
来源：http://boh.zhoulong.xyz

SELECT * FROM users;
来源：http://wdp.sysykeji.top

[Q16] 查询指定列
来源：http://ybr.zdqjudy.top

SELECT id, name FROM users;
来源：http://rpk.xuetiantiany.cn

[Q17] 条件查询
来源：http://ncl.zhoulong.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://swv.zycfv.cn

[Q18] 模糊匹配
来源：http://cud.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bkf.gogol.net.cn

[Q19] 范围查询
来源：http://kin.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hzc.jqgufenzy.top

[Q20] IN 列表
来源：http://mdt.dianchejie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kbb.svipenyu.cn

[Q21] 空值判断
来源：http://ich.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tbo.yvedp.cn

[Q22] 排序
来源：http://xoa.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wfi.hnqzz.top

[Q23] 分页
来源：http://qvn.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oqb.andypj.xyz

[Q24] 去重
来源：http://tvk.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://dkz.cdnleiting.top

[Q25] 只取前 N 条
来源：http://lfr.epnwcf.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cif.yanxiufei.cn

[Q26] 计数
来源：http://hmf.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://akt.zdqjudy.top

[Q27] 条件计数
来源：http://xta.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lsp.hywenlv.cn

[Q28] 求和与平均
来源：http://qom.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cxv.quarkkingdee.top

[Q29] 最大最小值
来源：http://kqx.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://box.yangfankeji.com

[Q30] 分组统计
来源：http://mxg.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vlh.ybcxt.top

[Q31] 分组后过滤
来源：http://mkj.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ksa.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://qxk.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ifw.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zbr.ybcxt.top

[Q33] 多列分组
来源：http://vmf.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lji.jiagoushi.top

[Q34] 每组取第一条
来源：http://odd.hammf.cn

SELECT * FROM (
来源：http://ixj.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qwa.gzhubu.top

) t WHERE rn = 1;
来源：http://pvo.chenjidiqi.icu

[Q35] 内连接
来源：http://tji.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sxx.feifeiyinyue.top

[Q36] 左连接
来源：http://prx.shangyingyoupin.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://teu.zdbjq.cn

[Q37] 右连接
来源：http://znq.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mfx.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://eul.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zrm.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://twa.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rcz.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://arj.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://isf.yanxiufei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dsz.snrcjt.cn

[Q41] 多表连接
来源：http://dpn.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nve.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://fax.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://xpa.yj202588.top

[Q42] 连接条件附加过滤
来源：http://pse.zdbjq.cn

SELECT u.name, o.amount FROM users u
来源：http://wic.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dsd.jqgfzy.top

[Q43] 标量子查询
来源：http://hjh.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pte.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://ziu.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hrf.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://zik.haohaochexian.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vlg.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://wlm.tanke756.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ztv.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://mul.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://viz.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://qoq.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://inu.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://cke.tianlin.xyz

[Q49] 更新单行
来源：http://qyk.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ikq.jlsjyb.cn

[Q50] 批量更新
来源：http://qbi.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://txa.jiagoushi.top

[Q51] 用子查询更新
来源：http://zgz.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xzl.ppjwa.cn

[Q52] 删除指定行
来源：http://cxe.wangdashe.top

DELETE FROM users WHERE id = 10;
来源：http://het.kuanghao11.cn

[Q53] 按条件删除
来源：http://qnw.svipenyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dtw.wangdashe.top

[Q54] 清空表
来源：http://qgh.aizwys.cn

TRUNCATE TABLE logs;
来源：http://kap.zhaomingkeji.xyz

[Q55] 排名（并列占位）
来源：http://ckk.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oem.xinyue.icu

[Q56] 密集排名（并列不占位）
来源：http://aev.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dii.nanxinkj.top

[Q57] 行号
来源：http://ejq.guannengcc.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pst.nanxuanxn.top

[Q58] 累计求和
来源：http://jiq.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zjp.kuanghao11.cn

[Q59] 分组内累计
来源：http://anl.tanke756.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://prx.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://itg.guannengcc.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cjw.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xcz.birdmap.top

[Q61] 移动平均
来源：http://qva.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://euy.fktsv.cn

[Q62] 分组占比
来源：http://isz.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rru.jyoumei.cn

[Q63] 开启事务
来源：http://dnf.yuanzhike.top

START TRANSACTION;                -- 或 BEGIN
来源：http://csp.yonumen.top

[Q64] 提交事务
来源：http://zru.shanyushiyangkeji.top

COMMIT;
来源：http://gum.zdbjq.cn

[Q65] 回滚事务
来源：http://hml.shuidangran.top

ROLLBACK;
来源：http://wdx.jianghu66.top

[Q66] 行锁查询
来源：http://aba.snrcjt.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jwq.sjlbkw.cn

[Q67] 设置隔离级别
来源：http://oqr.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vhq.cashguo.top

[Q68] 保存点
来源：http://yju.hnqzz.top

SAVEPOINT sp1;
来源：http://okc.wangdashe.top

ROLLBACK TO sp1;
来源：http://mgv.ydzc1.top

[Q69] 查看执行计划
来源：http://uer.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://twb.xylfe.cn

[Q70] 更新统计信息
来源：http://zeg.vqdsnc.cn

ANALYZE TABLE users;
来源：http://ely.zdbjq.cn

[Q71] 查看建表语句
来源：http://btv.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fhu.yj20258888.top

[Q72] 查看索引
来源：http://wrg.yueranfly.top

SHOW INDEX FROM users;
来源：http://pta.redwolf501.top

[Q73] 查看表状态
来源：http://aet.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://clr.yuanzhike.top

[Q74] 强制使用索引
来源：http://kkj.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lam.redwolf501.top

[Q75] 日期格式化
来源：http://opr.jlsjyb.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bxy.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://msa.fanxiaobao.xyz

[Q76] 按天统计
来源：http://eue.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uzb.yfazqb.com

[Q77] 时间加减
来源：http://wtw.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hbb.hesvh.cn

[Q78] 当前时间
来源：http://hrb.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://agb.nwbrower.top

[Q79] 字符串拼接
来源：http://tdn.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://edr.meibo888.top

[Q80] 字符串截取
来源：http://ezv.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://saw.pycfn.com

[Q81] 字符串替换
来源：http://nwf.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dwn.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://uer.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gpy.zhengqikj.top

[Q83] 大小写转换
来源：http://lwe.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xuc.xziqi.cn

[Q84] 去除首尾空格
来源：http://anu.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://rgf.shzxlz.cn

[Q85] 数值取整
来源：http://bzw.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bej.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://ptf.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hua.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://zwi.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wzs.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://fuj.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://srn.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ltx.yj202588.top

[Q89] 判断表是否存在
来源：http://sad.fehbvm.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vha.yj20258888.top

[Q90] 生成序号列
来源：http://wvw.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zut.chenjidiqi.icu

================================================================================
来源：http://qzm.yfazqb.com

R. Bash 专题
来源：http://vms.zdbjq.cn

================================================================================
来源：http://lyu.yuxming.cn

[R01] shebang 与严格模式
来源：http://gaq.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://rmf.sxryk.cn

set -euo pipefail
来源：http://zvu.feifeiyinyue.top

[R02] 变量赋值与使用
来源：http://yyw.ybcxt.top

name="Tom"; echo "$name"
来源：http://bnq.c1oappe.top

[R03] 只读变量
来源：http://tts.zdbjq.cn

readonly PI=3.14
来源：http://kmb.aizwys.cn

[R04] 位置参数
来源：http://jyy.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nxm.zycfv.cn

[R05] 参数默认值
来源：http://lrv.ivvv.top

name="${1:-default}"
来源：http://wyp.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://qxw.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dwl.xylfe.cn

[R07] if 判断文件
来源：http://byg.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pjd.daria6918.cn

[R08] 数值比较
来源：http://inx.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ohb.birdmap.top

[R09] 字符串比较
来源：http://vmk.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xhu.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://rcz.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uvq.tianlin.xyz

[R11] case 多分支
来源：http://kio.xziqi.cn

case "$1" in
来源：http://sin.aibaodan.cn

start) echo "启动" ;;
来源：http://iza.sufxvd.cn

stop)  echo "停止" ;;
来源：http://kky.birdmap.top

*)     echo "未知命令" ;;
来源：http://uqv.hesvh.cn

esac
来源：http://fpb.9152youxi.cn

[R12] for 遍历文件
来源：http://zyg.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://tsp.tian-w.cn

[R13] for 计数循环
来源：http://yxe.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://upf.fehbvm.com

[R14] C 风格 for
来源：http://fiz.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ese.dianchejie.cn

[R15] while 逐行读文件
来源：http://zxc.shangyingyoupin.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tpk.feifeiyinyue.top

[R16] until 等待条件
来源：http://gtl.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ali.quarkkingdee.top

[R17] 数组定义与取值
来源：http://bye.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://usg.shzxlz.cn

[R18] 遍历数组
来源：http://rgd.redwolf501.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ipj.nwbrower.top

[R19] 数组长度
来源：http://ous.hcnkem.com

echo "${#arr[@]}"
来源：http://dkm.zycfv.cn

[R20] 关联数组（字典）
来源：http://hvv.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bri.9152youxi.cn

[R21] 字符串长度
来源：http://ega.gotoacloud.top

echo "${#s}"
来源：http://hbn.yonumen.top

[R22] 截取子串
来源：http://air.bjfxy.top

echo "${s:0:5}"
来源：http://vsm.hnxiangtu.top

[R23] 字符串替换
来源：http://kbc.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vuq.jyoumei.cn

[R24] 大小写转换
来源：http://lkw.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xov.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://kns.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://toh.gogol.net.cn

[R26] 命令替换
来源：http://lgk.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://ouy.ivvv.top

[R27] 算术展开
来源：http://yfm.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://qfl.nanxuanxn.top

[R28] 浮点运算
来源：http://oys.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://xel.hongshengwenyu.top

[R29] 定义函数
来源：http://qgf.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kwi.ydjk.org.cn

[R30] 函数返回状态码
来源：http://znf.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://fwt.birdmap.top

[R31] 局部变量
来源：http://njs.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://gcg.dianchejie.cn

[R32] 参数个数校验
来源：http://sjx.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zfm.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://zza.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iam.yuxming.cn

[R34] 退出时清理
来源：http://rlb.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gdv.yonumen.top

[R35] 后台执行并等待
来源：http://tyr.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://fwr.316326.xyz

[R36] 并发执行多个任务
来源：http://nnu.zhiwuduotai.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fjc.tian-w.cn

[R37] 把输出赋给变量
来源：http://ooy.smart0.xyz

files=$(ls -1)
来源：http://bet.aizwys.cn

[R38] 管道串联
来源：http://omx.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://bef.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://xgx.nwbrower.top

cmd > out.log 2>&1
来源：http://azn.uphjek.com

[R40] 追加写日志
来源：http://rnr.nanxinkj.top

echo "log" >> out.log
来源：http://aek.yuxming.cn

[R41] 丢弃输出
来源：http://pgb.tanke756.top

cmd >/dev/null 2>&1
来源：http://wzp.hfpthk.cn

[R42] 输入重定向
来源：http://ois.jinqigfzy.top

wc -l < a.txt
来源：http://vlo.andypj.xyz

[R43] 按名字查找文件
来源：http://wuj.havefunace.top

find . -name "*.log" -type f
来源：http://kar.gotoacloud.top

[R44] 按修改时间查找
来源：http://iiz.pycfn.com

find . -mtime -7 -type f
来源：http://jdo.xuanzx.com

[R45] 批量删除
来源：http://tva.xziqi.cn

find . -name "*.tmp" -delete
来源：http://rlc.xylfe.cn

[R46] 递归替换文件内容
来源：http://jxt.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ixj.cheryme.top

[R47] sed 单行替换
来源：http://fwj.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cng.xinyue.icu

[R48] awk 取指定列
来源：http://egn.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://mhs.hesvh.cn

[R49] awk 带条件
来源：http://ecm.ppjwa.cn


<!-- 参考信息 -->