代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://tgc.cdnleiting.top

[Q07] 删除表
来源：http://tdt.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://mdi.vqdsnc.cn

[Q08] 创建普通索引
来源：http://qgw.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uuy.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://mym.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rxq.yanxiufei.cn

[Q10] 插入单行
来源：http://wvd.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oxd.gogol.net.cn

[Q11] 一次插入多行
来源：http://lex.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gbo.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://lii.guannengcc.top

INSERT INTO users (name) VALUES ('C');
来源：http://ftt.yuxming.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ghq.jiagoushi.top

[Q13] 忽略重复插入
来源：http://fpz.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nob.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://ula.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aja.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vcj.xylfe.cn

[Q15] 查询全部
来源：http://rrn.nanxinkj.top

SELECT * FROM users;
来源：http://lvq.zhiwuduotai.top

[Q16] 查询指定列
来源：http://pfn.snrcjt.cn

SELECT id, name FROM users;
来源：http://isv.sweek.top

[Q17] 条件查询
来源：http://wso.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fep.yangfankeji.com

[Q18] 模糊匹配
来源：http://xsf.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cbz.gotoacloud.top

[Q19] 范围查询
来源：http://fwx.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vwz.sxryk.cn

[Q20] IN 列表
来源：http://adn.jqgfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yob.guowangkeji.top

[Q21] 空值判断
来源：http://hhc.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fra.yonumen.top

[Q22] 排序
来源：http://hyv.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fei.jinghuilouyu.cn

[Q23] 分页
来源：http://ten.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yqa.cqqwz.cn

[Q24] 去重
来源：http://vkw.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://uju.chenjidiqi.icu

[Q25] 只取前 N 条
来源：http://rdx.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wbh.gogol.net.cn

[Q26] 计数
来源：http://ttn.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://ckm.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://dog.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lnk.shuidangran.top

[Q28] 求和与平均
来源：http://fxl.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iix.yj20258.top

[Q29] 最大最小值
来源：http://kan.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://crb.fengsongda.top

[Q30] 分组统计
来源：http://lym.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wib.pycfn.com

[Q31] 分组后过滤
来源：http://ard.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uwx.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://oqs.yanxiufei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hvx.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://evm.haohaochexian.top

[Q33] 多列分组
来源：http://ibz.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vco.haohaochexian.top

[Q34] 每组取第一条
来源：http://gay.xziqi.cn

SELECT * FROM (
来源：http://wzf.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dbk.havefunace.top

) t WHERE rn = 1;
来源：http://heu.nwbrower.top

[Q35] 内连接
来源：http://nhp.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bek.shuidangran.top

[Q36] 左连接
来源：http://kmm.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nbs.chenjidiqi.icu

[Q37] 右连接
来源：http://wlu.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vkg.yanxiufei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://itb.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cji.fengsongda.top

[Q39] 自连接（查上下级）
来源：http://rze.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zwj.havefunace.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kgt.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://syh.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uio.nanxinkj.top

[Q41] 多表连接
来源：http://xvk.sufxvd.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bsq.bbcook.cn

JOIN users u ON u.id = o.user_id
来源：http://fuk.cashguo.top

JOIN products p ON p.id = o.product_id;
来源：http://ljg.meibo888.top

[Q42] 连接条件附加过滤
来源：http://yse.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://fcd.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ufy.zycfv.cn

[Q43] 标量子查询
来源：http://pik.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sib.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://ijh.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zbx.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://aij.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fca.pengpengdd.cyou

[Q46] NOT EXISTS 判断不存在
来源：http://muy.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oox.aizwys.cn

[Q47] 与平均值比较
来源：http://afc.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cpf.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://cyu.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ata.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://pdd.uphjek.com

[Q49] 更新单行
来源：http://urw.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yys.chenjidiqi.icu

[Q50] 批量更新
来源：http://bok.xylfe.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zht.nanxuanxn.top

[Q51] 用子查询更新
来源：http://bmx.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mew.hysaishi.cn

[Q52] 删除指定行
来源：http://lbq.birdmap.top

DELETE FROM users WHERE id = 10;
来源：http://xoy.jyoumei.cn

[Q53] 按条件删除
来源：http://oxm.xingfuxueyuan.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://viv.bbcook.cn

[Q54] 清空表
来源：http://cxq.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://ifc.jinqigufen.top

[Q55] 排名（并列占位）
来源：http://ooh.shanyushiyangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://stp.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://fqt.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uvd.gaohongyu789.top

[Q57] 行号
来源：http://djt.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yiz.hnqzz.top

[Q58] 累计求和
来源：http://cth.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xen.hfpthk.cn

[Q59] 分组内累计
来源：http://abz.ybcxt.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nrr.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://ybf.pengpengdd.cyou

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fbv.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yqt.daria6918.cn

[Q61] 移动平均
来源：http://fje.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yke.hnxiangtu.top

[Q62] 分组占比
来源：http://aqi.chenlongwang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vpp.cqqwz.cn

[Q63] 开启事务
来源：http://coz.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://tga.ydzc1.top

[Q64] 提交事务
来源：http://azf.jyoumei.cn

COMMIT;
来源：http://nwg.pengpengdd.cyou

[Q65] 回滚事务
来源：http://yqy.cdnleiting.top

ROLLBACK;
来源：http://fcg.zycfv.cn

[Q66] 行锁查询
来源：http://asu.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://chl.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://lfg.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fmv.yvedp.cn

[Q68] 保存点
来源：http://jol.cqqwz.cn

SAVEPOINT sp1;
来源：http://wyk.daria6918.cn

ROLLBACK TO sp1;
来源：http://och.cdnleiting.top

[Q69] 查看执行计划
来源：http://opl.zhijiandao.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vto.ehwqpu.com

[Q70] 更新统计信息
来源：http://mvg.chenzaomai.com

ANALYZE TABLE users;
来源：http://bqm.aibaodan.cn

[Q71] 查看建表语句
来源：http://mai.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xqm.snrcjt.cn

[Q72] 查看索引
来源：http://aho.yj20258.top

SHOW INDEX FROM users;
来源：http://mjb.gzhubu.top

[Q73] 查看表状态
来源：http://rco.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qxq.xziqi.cn

[Q74] 强制使用索引
来源：http://heo.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rcu.daxiang520.top

[Q75] 日期格式化
来源：http://ecv.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://leu.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gpg.yongpay.top

[Q76] 按天统计
来源：http://svb.jianghu66.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uit.birdmap.top

[Q77] 时间加减
来源：http://zlm.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tsy.dianchejie.cn

[Q78] 当前时间
来源：http://bmu.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sav.kuanghao11.cn

[Q79] 字符串拼接
来源：http://fzr.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jvq.nanxinkj.top

[Q80] 字符串截取
来源：http://zvk.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gsf.shangyingyoupin.top

[Q81] 字符串替换
来源：http://ufq.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fcp.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://gsr.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mlw.aibaodan.cn

[Q83] 大小写转换
来源：http://cef.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vzt.sxryk.cn

[Q84] 去除首尾空格
来源：http://hhh.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://erv.pycfn.com

[Q85] 数值取整
来源：http://hnl.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zwt.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://wom.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kkk.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://fjd.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gjy.fengsongda.top

[Q88] 行转列（条件聚合）
来源：http://xdn.hongshengwenyu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fgg.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vjl.tarul.cn

[Q89] 判断表是否存在
来源：http://arq.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://icm.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://kor.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lly.sxryk.cn

================================================================================
来源：http://njy.hammf.cn

R. Bash 专题
来源：http://rnx.jqgfzy.top

================================================================================
来源：http://ups.xuanzx.com

[R01] shebang 与严格模式
来源：http://mdl.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://guc.nanxuanxn.top

set -euo pipefail
来源：http://yne.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://eli.hcnkem.com

name="Tom"; echo "$name"
来源：http://giz.quarkkingdee.top

[R03] 只读变量
来源：http://uwm.cashguo.top

readonly PI=3.14
来源：http://boo.c1oappe.top

[R04] 位置参数
来源：http://xgz.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ljn.yuxming.cn

[R05] 参数默认值
来源：http://nwz.quarkkingdee.top

name="${1:-default}"
来源：http://nqw.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://gyw.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://czh.tanke756.top

[R07] if 判断文件
来源：http://dec.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vkm.snrcjt.cn

[R08] 数值比较
来源：http://vew.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yng.iojbl.cn

[R09] 字符串比较
来源：http://wsv.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gkq.yangfankeji.com

[R10] 正则匹配
来源：http://elh.hesvh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hno.cashguo.top

[R11] case 多分支
来源：http://xux.vqdsnc.cn

case "$1" in
来源：http://mfi.zycfv.cn

start) echo "启动" ;;
来源：http://ugq.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://pys.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://oya.xylfe.cn

esac
来源：http://vzk.shangyingyoupin.top

[R12] for 遍历文件
来源：http://qby.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://mfa.tanke756.top

[R13] for 计数循环
来源：http://bcb.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://eow.52xcode.cn

[R14] C 风格 for
来源：http://xsz.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ens.tianlin.xyz

[R15] while 逐行读文件
来源：http://lmn.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pbq.ivvv.top

[R16] until 等待条件
来源：http://ynj.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qgd.tarul.cn

[R17] 数组定义与取值
来源：http://voh.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://gsn.feifeiyinyue.top

[R18] 遍历数组
来源：http://qqm.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vdr.chenzaomai.com

[R19] 数组长度
来源：http://mar.sxryk.cn

echo "${#arr[@]}"
来源：http://unw.andypj.xyz

[R20] 关联数组（字典）
来源：http://xnl.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hxz.guowangkeji.top

[R21] 字符串长度
来源：http://clw.vehdjk.com

echo "${#s}"
来源：http://gdl.hysaishi.cn

[R22] 截取子串
来源：http://tdj.jinqigfzy.top

echo "${s:0:5}"
来源：http://wtn.shangyingyoupin.top

[R23] 字符串替换
来源：http://avd.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cvx.jyoumei.cn

[R24] 大小写转换
来源：http://jnw.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://iqx.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://nqe.iojbl.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mjx.ppjwa.cn

[R26] 命令替换
来源：http://eco.meibo888.top

now=$(date +%F); echo "$now"
来源：http://svu.52xcode.cn

[R27] 算术展开
来源：http://hpf.yuxming.cn

echo $((1 + 2 * 3))
来源：http://myw.bbcook.cn

[R28] 浮点运算
来源：http://uop.gaohongyu789.top

echo "scale=2; 10/3" | bc
来源：http://pzn.daxiang520.top

[R29] 定义函数
来源：http://mwm.kuanghao11.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mpq.tian-w.cn

[R30] 函数返回状态码
来源：http://fnl.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://otw.dashuyun.cn

[R31] 局部变量
来源：http://pla.iojbl.cn

f() { local x=1; echo "$x"; }
来源：http://qny.xingfuxueyuan.xyz

[R32] 参数个数校验
来源：http://xqr.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sbi.pycfn.com

[R33] 捕获错误并提示行号
来源：http://ehi.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mum.uphjek.com

[R34] 退出时清理
来源：http://vfd.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://did.fengsongda.top

[R35] 后台执行并等待
来源：http://npl.snrcjt.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://szj.cashguo.top

[R36] 并发执行多个任务
来源：http://qyr.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tmt.cashguo.top

[R37] 把输出赋给变量
来源：http://ktf.hfpthk.cn

files=$(ls -1)
来源：http://gow.xuanzx.com

[R38] 管道串联
来源：http://yfp.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://kfy.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://fxc.bjfxy.top

cmd > out.log 2>&1
来源：http://agt.iojbl.cn

[R40] 追加写日志
来源：http://jvg.52xcode.cn

echo "log" >> out.log
来源：http://oih.sysykeji.top

[R41] 丢弃输出
来源：http://ius.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://urd.kuanghao11.cn

[R42] 输入重定向
来源：http://nza.sufxvd.cn

wc -l < a.txt
来源：http://pgr.ivvv.top

[R43] 按名字查找文件
来源：http://ihr.zhengqikj.top

find . -name "*.log" -type f
来源：http://ekm.gaohongyu789.top

[R44] 按修改时间查找
来源：http://hbt.hywenlv.cn

find . -mtime -7 -type f
来源：http://fxj.hywenlv.cn

[R45] 批量删除
来源：http://rge.ybcxt.top

find . -name "*.tmp" -delete
来源：http://tvr.hfpthk.cn

[R46] 递归替换文件内容
来源：http://ybg.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iwm.cdnleiting.top

[R47] sed 单行替换
来源：http://yxn.fehbvm.com

sed -i 's/foo/bar/g' a.txt
来源：http://zqg.havefunace.top

[R48] awk 取指定列
来源：http://qxo.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://kco.yfazqb.com

[R49] awk 带条件
来源：http://rag.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qux.fzhhl.top

[R50] awk 求和
来源：http://dal.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mrg.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://czc.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qxw.ehwqpu.com

[R52] 统计行数
来源：http://ztb.quarkkingdee.top

wc -l a.txt
来源：http://qyr.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://vvk.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rvx.chenjidiqi.icu

[R54] 比较两个文件
来源：http://ytg.ivvv.top

diff a.txt b.txt
来源：http://tdd.yj20258888.top

[R55] 压缩与解压
来源：http://xow.aizwys.cn


<!-- 参考信息 -->