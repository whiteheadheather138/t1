代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gyl.chenzaomai.com

[Q05] 重命名列
来源：http://nii.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ong.shanyushiyangtech.top

[Q06] 删除列
来源：http://voh.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ync.yueranfly.top

[Q07] 删除表
来源：http://zhf.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://tib.aizwys.cn

[Q08] 创建普通索引
来源：http://bfz.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oeb.cheryme.top

[Q09] 创建唯一索引
来源：http://siz.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lzj.quarkkingdee.top

[Q10] 插入单行
来源：http://wsx.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dbt.zhixingplan.top

[Q11] 一次插入多行
来源：http://fxv.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vdq.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://pws.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://ahm.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hay.sysykeji.top

[Q13] 忽略重复插入
来源：http://qnb.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qly.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://zug.xuetiantiany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mmi.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uya.zhiwuduotai.top

[Q15] 查询全部
来源：http://wam.gogol.net.cn

SELECT * FROM users;
来源：http://msq.jianghu66.top

[Q16] 查询指定列
来源：http://kjm.yongpay.top

SELECT id, name FROM users;
来源：http://sam.xylfe.cn

[Q17] 条件查询
来源：http://nra.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fkn.epnwcf.com

[Q18] 模糊匹配
来源：http://hfi.quarkkingdee.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hon.xziqi.cn

[Q19] 范围查询
来源：http://olt.gogol.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zcq.xinyue.icu

[Q20] IN 列表
来源：http://gwr.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xxa.chenlongwang.top

[Q21] 空值判断
来源：http://oia.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xma.cashguo.top

[Q22] 排序
来源：http://hte.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ikj.birdmap.top

[Q23] 分页
来源：http://mdi.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eoy.yfazqb.com

[Q24] 去重
来源：http://cke.yj202588.top

SELECT DISTINCT city FROM users;
来源：http://uqn.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://uul.jianghu66.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kop.316326.xyz

[Q26] 计数
来源：http://bto.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://npg.ehwqpu.com

[Q27] 条件计数
来源：http://kjg.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kkp.jiagoushi.top

[Q28] 求和与平均
来源：http://fhs.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eda.yuxming.cn

[Q29] 最大最小值
来源：http://uyd.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zrc.zhoulong.xyz

[Q30] 分组统计
来源：http://drp.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nsn.gotoacloud.top

[Q31] 分组后过滤
来源：http://bit.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lzo.316326.xyz

[Q32] 分组拼接字符串
来源：http://zqy.fengsongda.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nti.9152youxi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://znh.chenlongwang.top

[Q33] 多列分组
来源：http://dtp.shanyushiyangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nic.fktsv.cn

[Q34] 每组取第一条
来源：http://djw.hysaishi.cn

SELECT * FROM (
来源：http://yqk.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ntp.kuanghao11.cn

) t WHERE rn = 1;
来源：http://myh.tanke756.top

[Q35] 内连接
来源：http://qta.redwolf501.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hxe.daria6918.cn

[Q36] 左连接
来源：http://cmh.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kjf.meibo888.top

[Q37] 右连接
来源：http://aos.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rdo.jlsjyb.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ikd.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://koy.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://aby.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zqf.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cej.zhoulong.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://njk.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jkv.gzhubu.top

[Q41] 多表连接
来源：http://otc.quarkkingdee.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mqq.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://asw.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://azs.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://vat.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://std.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ldy.dashuyun.cn

[Q43] 标量子查询
来源：http://syj.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mkp.zycfv.cn

[Q44] IN 子查询
来源：http://ulp.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ypl.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://nuq.zhaomingkeji.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jls.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://und.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dsv.jinqigufen.top

[Q47] 与平均值比较
来源：http://zyx.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uol.ydjk.org.cn

[Q48] CTE 公用表表达式
来源：http://mmk.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wrh.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://mlr.yongpay.top

[Q49] 更新单行
来源：http://gmt.jyoumei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://keu.chenzaomai.com

[Q50] 批量更新
来源：http://rhp.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iin.fktsv.cn

[Q51] 用子查询更新
来源：http://kqj.kuanghao11.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uxi.xinyue.icu

[Q52] 删除指定行
来源：http://tor.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://xuv.yvedp.cn

[Q53] 按条件删除
来源：http://ssa.zhijiandao.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ecz.9152youxi.cn

[Q54] 清空表
来源：http://nux.xuanzx.com

TRUNCATE TABLE logs;
来源：http://ekp.cheryme.top

[Q55] 排名（并列占位）
来源：http://ozi.cqqwz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hzt.fanxiaobao.xyz

[Q56] 密集排名（并列不占位）
来源：http://wsw.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xok.zhaomingkeji.xyz

[Q57] 行号
来源：http://hpl.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rhu.tianlin.xyz

[Q58] 累计求和
来源：http://ghu.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wvv.aizwys.cn

[Q59] 分组内累计
来源：http://esc.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dcy.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://hhb.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://itc.yj20258888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cvg.bjfxy.top

[Q61] 移动平均
来源：http://tfy.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uye.shuidangran.top

[Q62] 分组占比
来源：http://hqv.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jpn.zhoulong.xyz

[Q63] 开启事务
来源：http://ppj.snrcjt.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bcg.c1oappe.top

[Q64] 提交事务
来源：http://jqi.hammf.cn

COMMIT;
来源：http://mtq.chenjidiqi.icu

[Q65] 回滚事务
来源：http://qnf.fzhhl.top

ROLLBACK;
来源：http://pkj.chenjidiqi.icu

[Q66] 行锁查询
来源：http://pcu.ydzc1.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tez.birdmap.top

[Q67] 设置隔离级别
来源：http://hcp.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rpc.zhongyouzk.top

[Q68] 保存点
来源：http://nia.0kj1m.cn

SAVEPOINT sp1;
来源：http://dwb.hysaishi.cn

ROLLBACK TO sp1;
来源：http://vgv.zhongyouzk.top

[Q69] 查看执行计划
来源：http://irg.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xwt.sufxvd.cn

[Q70] 更新统计信息
来源：http://qot.zhengqikj.top

ANALYZE TABLE users;
来源：http://sib.gogol.net.cn

[Q71] 查看建表语句
来源：http://xpp.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ish.nwbrower.top

[Q72] 查看索引
来源：http://ali.birdmap.top

SHOW INDEX FROM users;
来源：http://uoa.jiagoushi.top

[Q73] 查看表状态
来源：http://zvl.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mij.yueranfly.top

[Q74] 强制使用索引
来源：http://mcg.hcnkem.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cay.zycfv.cn

[Q75] 日期格式化
来源：http://cxk.gaohongyu789.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lok.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lwr.0kj1m.cn

[Q76] 按天统计
来源：http://ejx.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sqf.yuanzhike.top

[Q77] 时间加减
来源：http://ggh.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xlw.quarkkingdee.top

[Q78] 当前时间
来源：http://bxa.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fha.quarkkingdee.top

[Q79] 字符串拼接
来源：http://oed.guowangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jby.fengsongda.top

[Q80] 字符串截取
来源：http://xtj.hcnkem.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ztz.shangyingyoupin.top

[Q81] 字符串替换
来源：http://fyn.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mbn.yj202588.top

[Q82] 字符长度与字节长度
来源：http://ytm.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xsa.shangyingyoupin.top

[Q83] 大小写转换
来源：http://qyj.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ijb.tarul.cn

[Q84] 去除首尾空格
来源：http://lxx.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://evb.chenzaomai.com

[Q85] 数值取整
来源：http://qku.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xuy.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://vah.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mcj.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://dmz.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kdn.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://wbb.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ixz.meibo888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uew.xylfe.cn

[Q89] 判断表是否存在
来源：http://myi.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lia.xziqi.cn

[Q90] 生成序号列
来源：http://fcw.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hxk.jinqigfzy.top

================================================================================
来源：http://utc.chenjidiqi.icu

R. Bash 专题
来源：http://ycx.smart0.xyz

================================================================================
来源：http://umg.xuanzx.com

[R01] shebang 与严格模式
来源：http://msr.yueranfly.top

#!/usr/bin/env bash
来源：http://spe.yj202588.top

set -euo pipefail
来源：http://lpn.haohaochexian.top

[R02] 变量赋值与使用
来源：http://eed.ppjwa.cn

name="Tom"; echo "$name"
来源：http://apx.pycfn.com

[R03] 只读变量
来源：http://ame.jinqigufen.top

readonly PI=3.14
来源：http://nqk.shzxlz.cn

[R04] 位置参数
来源：http://adq.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nsd.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://fqy.fktsv.cn

name="${1:-default}"
来源：http://vsp.hammf.cn

[R06] 判断命令是否存在
来源：http://cpq.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tqy.zhoulong.xyz

[R07] if 判断文件
来源：http://yhq.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tnz.wangdashe.top

[R08] 数值比较
来源：http://mzv.zdqjudy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ruw.dianchejie.cn

[R09] 字符串比较
来源：http://qyq.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dst.hfpthk.cn

[R10] 正则匹配
来源：http://ahs.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aed.shanyushiyangkeji.top

[R11] case 多分支
来源：http://wbd.cucudq.cn

case "$1" in
来源：http://hhv.jianghu66.top

start) echo "启动" ;;
来源：http://gmu.hesvh.cn

stop)  echo "停止" ;;
来源：http://prc.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://atv.jinqigfzy.top

esac
来源：http://rni.0kj1m.cn

[R12] for 遍历文件
来源：http://fdj.zhiwuduotai.top

for f in *.txt; do echo "$f"; done
来源：http://kfe.hywenlv.cn

[R13] for 计数循环
来源：http://nck.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://lbx.yuanzhike.top

[R14] C 风格 for
来源：http://zbd.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lsr.birdmap.top

[R15] while 逐行读文件
来源：http://caj.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mci.uphjek.com

[R16] until 等待条件
来源：http://dya.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dve.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://ype.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://qvy.guannengcc.top

[R18] 遍历数组
来源：http://lmh.andypj.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nhh.fktsv.cn

[R19] 数组长度
来源：http://irj.cucudq.cn

echo "${#arr[@]}"
来源：http://pya.hongshengwenyu.top

[R20] 关联数组（字典）
来源：http://dud.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dhi.bbcook.cn

[R21] 字符串长度
来源：http://ftw.ctjpmb.com

echo "${#s}"
来源：http://rvi.gogol.net.cn

[R22] 截取子串
来源：http://ong.meibo888.top

echo "${s:0:5}"
来源：http://nwy.daxiang520.top

[R23] 字符串替换
来源：http://ljb.fzhhl.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zqg.wangshuangyany.cn

[R24] 大小写转换
来源：http://bfn.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kdm.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://tbw.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jhi.vqdsnc.cn

[R26] 命令替换
来源：http://rex.zhijiandao.cn

now=$(date +%F); echo "$now"
来源：http://tni.52xcode.cn

[R27] 算术展开
来源：http://mmr.yvedp.cn

echo $((1 + 2 * 3))
来源：http://xpp.zdbjq.cn

[R28] 浮点运算
来源：http://rxu.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://clw.fehbvm.com

[R29] 定义函数
来源：http://kzy.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dxm.hysaishi.cn

[R30] 函数返回状态码
来源：http://arp.ydjk.org.cn

f() { return 0; }; f || echo "失败了"
来源：http://dih.vehdjk.com

[R31] 局部变量
来源：http://wwk.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://awy.0kj1m.cn

[R32] 参数个数校验
来源：http://bzz.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zvm.yj202588.top

[R33] 捕获错误并提示行号
来源：http://dkl.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rkk.jqgfzy.top

[R34] 退出时清理
来源：http://mzg.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wsa.shuidangran.top

[R35] 后台执行并等待
来源：http://sxk.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nbc.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://eih.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eqb.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://ndo.gzhubu.top

files=$(ls -1)
来源：http://hyf.jinghuilouyu.cn

[R38] 管道串联
来源：http://can.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://nzp.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://ruf.svipenyu.cn

cmd > out.log 2>&1
来源：http://goh.feifeiyinyue.top

[R40] 追加写日志
来源：http://htp.snrcjt.cn

echo "log" >> out.log
来源：http://vhh.fzhhl.top

[R41] 丢弃输出
来源：http://wco.yj20258888.top

cmd >/dev/null 2>&1
来源：http://yee.bbcook.cn

[R42] 输入重定向
来源：http://sjy.ydjk.org.cn

wc -l < a.txt
来源：http://eed.smart0.xyz

[R43] 按名字查找文件
来源：http://djd.sjlbkw.cn

find . -name "*.log" -type f
来源：http://pad.pycfn.com

[R44] 按修改时间查找
来源：http://voe.shzxlz.cn

find . -mtime -7 -type f
来源：http://edg.daxiang520.top

[R45] 批量删除
来源：http://afl.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://max.hfpthk.cn

[R46] 递归替换文件内容
来源：http://ebn.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gle.hesvh.cn

[R47] sed 单行替换
来源：http://dos.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://isb.c1oappe.top

[R48] awk 取指定列
来源：http://mmt.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://tix.snrcjt.cn

[R49] awk 带条件
来源：http://csr.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pkp.bbcook.cn

[R50] awk 求和
来源：http://pdq.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cgv.hywenlv.cn

[R51] 排序去重取前几
来源：http://wdo.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://msn.jqgfzy.top

[R52] 统计行数
来源：http://wzr.ivvv.top

wc -l a.txt
来源：http://ztx.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://ilj.sysykeji.top


<!-- 参考信息 -->