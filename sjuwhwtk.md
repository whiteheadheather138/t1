代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://dpa.hammf.cn

[Q09] 创建唯一索引
来源：http://oyr.jinghuilouyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jll.shzxlz.cn

[Q10] 插入单行
来源：http://fgh.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kld.guannengcc.top

[Q11] 一次插入多行
来源：http://lmb.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dkd.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://zbw.xylfe.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gfu.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jfe.pycfn.com

[Q13] 忽略重复插入
来源：http://elg.vqdsnc.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xls.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://oow.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hkv.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bsj.yonumen.top

[Q15] 查询全部
来源：http://lxn.snrcjt.cn

SELECT * FROM users;
来源：http://imc.pycfn.com

[Q16] 查询指定列
来源：http://rlz.tian-w.cn

SELECT id, name FROM users;
来源：http://cni.aizwys.cn

[Q17] 条件查询
来源：http://lfc.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xtu.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://gbc.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mab.hysaishi.cn

[Q19] 范围查询
来源：http://phf.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zoa.chenlongwang.top

[Q20] IN 列表
来源：http://eju.jqgfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mcj.cqqwz.cn

[Q21] 空值判断
来源：http://jvc.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rhf.ywan-chungtsiang.top

[Q22] 排序
来源：http://hqr.jlsjyb.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dyh.yj20258.top

[Q23] 分页
来源：http://zco.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eea.pengpengdd.cyou

[Q24] 去重
来源：http://ejr.shanyushiyangtech.top

SELECT DISTINCT city FROM users;
来源：http://kzo.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://mtr.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mxk.yanxiufei.cn

[Q26] 计数
来源：http://kov.hcnkem.com

SELECT COUNT(*) FROM users;
来源：http://iyz.svipenyu.cn

[Q27] 条件计数
来源：http://eti.zhengqikj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nub.jinghuilouyu.cn

[Q28] 求和与平均
来源：http://syy.aibaodan.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pbu.cdnleiting.top

[Q29] 最大最小值
来源：http://nht.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hed.shzxlz.cn

[Q30] 分组统计
来源：http://nsm.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hll.fehbvm.com

[Q31] 分组后过滤
来源：http://xuw.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://huf.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://kdt.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fxi.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jis.zhijiandao.cn

[Q33] 多列分组
来源：http://xxb.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qml.xuanzx.com

[Q34] 每组取第一条
来源：http://pyj.ydjk.org.cn

SELECT * FROM (
来源：http://wmk.sxryk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kdx.fehbvm.com

) t WHERE rn = 1;
来源：http://hwn.zhixingplan.top

[Q35] 内连接
来源：http://ihf.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vhd.daxiang520.top

[Q36] 左连接
来源：http://tcl.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://svk.cdnleiting.top

[Q37] 右连接
来源：http://omp.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zxn.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://bcj.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kzm.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://gkb.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ebh.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://clw.yvedp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mif.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xcb.xylfe.cn

[Q41] 多表连接
来源：http://gzl.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ymh.guannengcc.top

JOIN users u ON u.id = o.user_id
来源：http://khy.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://vyc.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://fyy.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://rtm.zhongyouzk.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lzg.guannengcc.top

[Q43] 标量子查询
来源：http://ppr.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://roi.xuetiantiany.cn

[Q44] IN 子查询
来源：http://rub.bjfxy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://thi.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://kke.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wai.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://oeb.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wvt.fengsongda.top

[Q47] 与平均值比较
来源：http://nvl.yj20258888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gyy.gogol.net.cn

[Q48] CTE 公用表表达式
来源：http://vmq.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wee.shuidangran.top

SELECT * FROM t WHERE c > 5;
来源：http://zao.chenzaomai.com

[Q49] 更新单行
来源：http://rhl.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vmn.hnqzz.top

[Q50] 批量更新
来源：http://gdq.zycfv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ojs.shuidangran.top

[Q51] 用子查询更新
来源：http://mxb.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pjn.guowangkeji.top

[Q52] 删除指定行
来源：http://bjh.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://rvz.yfazqb.com

[Q53] 按条件删除
来源：http://iud.jlsjyb.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rbc.aizwys.cn

[Q54] 清空表
来源：http://klg.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://qcc.smart0.xyz

[Q55] 排名（并列占位）
来源：http://xmg.yj202588.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oto.jiagoushi.top

[Q56] 密集排名（并列不占位）
来源：http://zvr.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://djm.wangshuangyany.cn

[Q57] 行号
来源：http://rnx.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pbr.52xcode.cn

[Q58] 累计求和
来源：http://efo.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qxv.snrcjt.cn

[Q59] 分组内累计
来源：http://fow.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hnr.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://epx.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://opa.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://che.shuidangran.top

[Q61] 移动平均
来源：http://ruh.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zff.hnqzz.top

[Q62] 分组占比
来源：http://wqy.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ufw.zycfv.cn

[Q63] 开启事务
来源：http://ivl.wangdashe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gbt.gaohongyu789.top

[Q64] 提交事务
来源：http://aba.chenzaomai.com

COMMIT;
来源：http://tyh.bjfxy.top

[Q65] 回滚事务
来源：http://oea.sufxvd.cn

ROLLBACK;
来源：http://mey.vqdsnc.cn

[Q66] 行锁查询
来源：http://spa.yonumen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zye.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://vld.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wlj.nanxinkj.top

[Q68] 保存点
来源：http://sbd.cheryme.top

SAVEPOINT sp1;
来源：http://mpz.yangfankeji.com

ROLLBACK TO sp1;
来源：http://syn.52xcode.cn

[Q69] 查看执行计划
来源：http://yqc.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wvt.yongpay.top

[Q70] 更新统计信息
来源：http://tlu.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://jrd.fehbvm.com

[Q71] 查看建表语句
来源：http://hwo.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lqd.chenlongwang.top

[Q72] 查看索引
来源：http://mvn.sxryk.cn

SHOW INDEX FROM users;
来源：http://lof.hnxiangtu.top

[Q73] 查看表状态
来源：http://vup.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cxm.xinyue.icu

[Q74] 强制使用索引
来源：http://bmh.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dqs.bbcook.cn

[Q75] 日期格式化
来源：http://npr.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qch.cashguo.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wkf.bbcook.cn

[Q76] 按天统计
来源：http://icp.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ydn.c1oappe.top

[Q77] 时间加减
来源：http://ask.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yrv.ppjwa.cn

[Q78] 当前时间
来源：http://hjg.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lky.jinqigfzy.top

[Q79] 字符串拼接
来源：http://knz.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://agh.ybcxt.top

[Q80] 字符串截取
来源：http://cla.c1oappe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tjs.hammf.cn

[Q81] 字符串替换
来源：http://tch.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hei.yj20258888.top

[Q82] 字符长度与字节长度
来源：http://qzf.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jwi.zhoulong.xyz

[Q83] 大小写转换
来源：http://rww.hysaishi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lsn.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://dwy.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://syb.yangfankeji.com

[Q85] 数值取整
来源：http://xhf.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ivz.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://rjn.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hcp.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://ben.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ckv.jinqigufen.top

[Q88] 行转列（条件聚合）
来源：http://ewp.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ahc.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mco.tarul.cn

[Q89] 判断表是否存在
来源：http://bis.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://erz.chenlongwang.top

[Q90] 生成序号列
来源：http://tfe.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vbv.tarul.cn

================================================================================
来源：http://svu.jqgufenzy.top

R. Bash 专题
来源：http://fjv.fehbvm.com

================================================================================
来源：http://nle.hcnkem.com

[R01] shebang 与严格模式
来源：http://ias.svipenyu.cn

#!/usr/bin/env bash
来源：http://zhe.zhoulong.xyz

set -euo pipefail
来源：http://knn.xinyue.icu

[R02] 变量赋值与使用
来源：http://sux.andypj.xyz

name="Tom"; echo "$name"
来源：http://atc.dashuyun.cn

[R03] 只读变量
来源：http://hug.ybcxt.top

readonly PI=3.14
来源：http://lvx.ybcxt.top

[R04] 位置参数
来源：http://bho.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fkj.daria6918.cn

[R05] 参数默认值
来源：http://jxl.shangyingyoupin.top

name="${1:-default}"
来源：http://dpg.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://vfl.cqqwz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vxr.yueranfly.top

[R07] if 判断文件
来源：http://vka.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hps.redwolf501.top

[R08] 数值比较
来源：http://uaf.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://eiq.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://myy.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://scw.ivvv.top

[R10] 正则匹配
来源：http://lmh.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fas.zycfv.cn

[R11] case 多分支
来源：http://vpa.sjlbkw.cn

case "$1" in
来源：http://tvp.fehbvm.com

start) echo "启动" ;;
来源：http://aac.xziqi.cn

stop)  echo "停止" ;;
来源：http://fac.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://lvd.yj20258888.top

esac
来源：http://isl.birdmap.top

[R12] for 遍历文件
来源：http://lqw.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://rbd.bjfxy.top

[R13] for 计数循环
来源：http://ufz.ctjpmb.com

for i in {1..10}; do echo "$i"; done
来源：http://ipn.jinqigfzy.top

[R14] C 风格 for
来源：http://mag.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oap.vehdjk.com

[R15] while 逐行读文件
来源：http://wpd.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bxf.ctjpmb.com

[R16] until 等待条件
来源：http://lmj.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dqf.redwolf501.top

[R17] 数组定义与取值
来源：http://kxo.bbcook.cn

arr=(a b c); echo "${arr[0]}"
来源：http://clr.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://yth.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fxi.kuanghao11.cn

[R19] 数组长度
来源：http://nvh.yj202588.top

echo "${#arr[@]}"
来源：http://eme.andypj.xyz

[R20] 关联数组（字典）
来源：http://fac.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zqd.cashguo.top

[R21] 字符串长度
来源：http://lpy.jinqigfzy.top

echo "${#s}"
来源：http://kkg.gzhubu.top

[R22] 截取子串
来源：http://cgh.9152youxi.cn

echo "${s:0:5}"
来源：http://zwg.zhoulong.xyz

[R23] 字符串替换
来源：http://liu.jlsjyb.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ifq.zhengqikj.top

[R24] 大小写转换
来源：http://sjt.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://oet.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://exd.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dgz.cdnleiting.top

[R26] 命令替换
来源：http://tox.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://ice.daria6918.cn

[R27] 算术展开
来源：http://rou.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://vce.epnwcf.com

[R28] 浮点运算
来源：http://gfc.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://tpb.meibo888.top

[R29] 定义函数
来源：http://zap.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xhx.yuanzhike.top

[R30] 函数返回状态码
来源：http://bvi.ybcxt.top

f() { return 0; }; f || echo "失败了"
来源：http://tff.sysykeji.top

[R31] 局部变量
来源：http://ftu.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://xll.jqgufenzy.top

[R32] 参数个数校验
来源：http://fhf.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://izv.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://aln.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ptc.nanxuanxn.top

[R34] 退出时清理
来源：http://psn.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dzt.sjlbkw.cn

[R35] 后台执行并等待
来源：http://aej.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vha.yj202588.top

[R36] 并发执行多个任务
来源：http://azl.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ohw.andypj.xyz

[R37] 把输出赋给变量
来源：http://jyn.hcnkem.com

files=$(ls -1)
来源：http://naq.yueranfly.top

[R38] 管道串联
来源：http://pbt.xziqi.cn

cat a.txt | grep -i error | wc -l
来源：http://wzv.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://prg.zycfv.cn

cmd > out.log 2>&1
来源：http://wdj.ctjpmb.com

[R40] 追加写日志
来源：http://hgt.jinqigufen.top

echo "log" >> out.log
来源：http://ayp.hnqzz.top

[R41] 丢弃输出
来源：http://gbp.316326.xyz

cmd >/dev/null 2>&1
来源：http://dui.gaohongyu789.top

[R42] 输入重定向
来源：http://jsb.guowangkeji.top

wc -l < a.txt
来源：http://tfv.ivvv.top

[R43] 按名字查找文件
来源：http://rva.jinqigufen.top

find . -name "*.log" -type f
来源：http://cio.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://sus.quarkkingdee.top

find . -mtime -7 -type f
来源：http://fmv.chenzaomai.com

[R45] 批量删除
来源：http://qtp.bbcook.cn

find . -name "*.tmp" -delete
来源：http://qto.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://dqi.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fcb.jinqigufen.top

[R47] sed 单行替换
来源：http://six.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ttf.daria6918.cn

[R48] awk 取指定列
来源：http://btz.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://nob.9152youxi.cn

[R49] awk 带条件
来源：http://szk.yuanzhike.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://czt.mhx1999.top

[R50] awk 求和
来源：http://ikj.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dod.daria6918.cn

[R51] 排序去重取前几
来源：http://esj.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://utt.birdmap.top

[R52] 统计行数
来源：http://ejh.zdqjudy.top

wc -l a.txt
来源：http://lto.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://ogr.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://smy.sjlbkw.cn

[R54] 比较两个文件
来源：http://acm.nanxuanxn.top

diff a.txt b.txt
来源：http://npk.zhoulong.xyz

[R55] 压缩与解压
来源：http://szd.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ryz.cdnleiting.top

[R56] 远程拷贝
来源：http://zqm.cheryme.top

scp file user@host:/path/
来源：http://ktn.chenlongwang.top

[R57] 远程执行命令
来源：http://qba.xylfe.cn


<!-- 参考信息 -->