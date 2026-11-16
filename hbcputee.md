代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yqg.nanxinkj.top

[Q11] 一次插入多行
来源：http://fuv.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xiv.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://huh.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://qnf.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tjo.ivvv.top

[Q13] 忽略重复插入
来源：http://abi.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ifv.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://cae.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rwj.sysykeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vyr.chenzaomai.com

[Q15] 查询全部
来源：http://xgk.daria6918.cn

SELECT * FROM users;
来源：http://sfa.tanke756.top

[Q16] 查询指定列
来源：http://tvk.aibaodan.cn

SELECT id, name FROM users;
来源：http://eyy.pengpengdd.cyou

[Q17] 条件查询
来源：http://sjk.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qiz.yongpay.top

[Q18] 模糊匹配
来源：http://ved.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ikt.hnqzz.top

[Q19] 范围查询
来源：http://mzo.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://phh.c1oappe.top

[Q20] IN 列表
来源：http://man.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ary.c1oappe.top

[Q21] 空值判断
来源：http://mvo.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bye.cdnleiting.top

[Q22] 排序
来源：http://ylj.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xzy.smart0.xyz

[Q23] 分页
来源：http://qej.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mad.pycfn.com

[Q24] 去重
来源：http://afx.cqqwz.cn

SELECT DISTINCT city FROM users;
来源：http://utj.cashguo.top

[Q25] 只取前 N 条
来源：http://djb.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ktj.wangdashe.top

[Q26] 计数
来源：http://dzu.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://ozq.sjlbkw.cn

[Q27] 条件计数
来源：http://ypj.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gsq.guowangkeji.top

[Q28] 求和与平均
来源：http://yvg.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://snf.52xcode.cn

[Q29] 最大最小值
来源：http://iue.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ubh.cdnleiting.top

[Q30] 分组统计
来源：http://jdo.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bru.xinyue.icu

[Q31] 分组后过滤
来源：http://qto.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ncp.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://pmn.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vrg.ywan-chungtsiang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hsy.chenlongwang.top

[Q33] 多列分组
来源：http://zrp.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lnl.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://nai.yueranfly.top

SELECT * FROM (
来源：http://dux.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xwh.ivvv.top

) t WHERE rn = 1;
来源：http://rhp.gaohongyu789.top

[Q35] 内连接
来源：http://juz.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pqg.fktsv.cn

[Q36] 左连接
来源：http://urs.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qjl.zhaomingkeji.xyz

[Q37] 右连接
来源：http://qpd.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bts.gzhubu.top

[Q38] 全外连接（PostgreSQL）
来源：http://svg.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cox.sxryk.cn

[Q39] 自连接（查上下级）
来源：http://xak.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://ugw.nwbrower.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fkp.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hqv.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yho.wangdashe.top

[Q41] 多表连接
来源：http://vtj.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://hyz.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://uke.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://yeh.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://rxy.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://hyu.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gvs.yj202588.top

[Q43] 标量子查询
来源：http://rkn.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jap.aibaodan.cn

[Q44] IN 子查询
来源：http://rlh.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://npr.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://wug.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rtk.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zgr.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nnn.yuxming.cn

[Q47] 与平均值比较
来源：http://bqb.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pcn.yonumen.top

[Q48] CTE 公用表表达式
来源：http://gmr.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rpp.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://rms.xuetiantiany.cn

[Q49] 更新单行
来源：http://zon.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://spz.birdmap.top

[Q50] 批量更新
来源：http://jzg.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yur.hysaishi.cn

[Q51] 用子查询更新
来源：http://jlk.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vmp.tian-w.cn

[Q52] 删除指定行
来源：http://kba.smart0.xyz

DELETE FROM users WHERE id = 10;
来源：http://iqo.xuanzx.com

[Q53] 按条件删除
来源：http://vli.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sik.0kj1m.cn

[Q54] 清空表
来源：http://ahz.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://ibp.hongshengwenyu.top

[Q55] 排名（并列占位）
来源：http://evc.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qwh.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://spj.yonumen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ftn.zhaomingkeji.xyz

[Q57] 行号
来源：http://tqr.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zwx.ehwqpu.com

[Q58] 累计求和
来源：http://qlw.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://drv.gotoacloud.top

[Q59] 分组内累计
来源：http://fvx.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hwo.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://jff.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mmq.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://myc.epnwcf.com

[Q61] 移动平均
来源：http://bbb.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sau.bbcook.cn

[Q62] 分组占比
来源：http://ipq.guannengcc.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vcw.shzxlz.cn

[Q63] 开启事务
来源：http://noz.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ldr.jqgfzy.top

[Q64] 提交事务
来源：http://snh.fehbvm.com

COMMIT;
来源：http://apw.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://rsp.haohaochexian.top

ROLLBACK;
来源：http://etr.yuxming.cn

[Q66] 行锁查询
来源：http://jgh.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uuq.hnxiangtu.top

[Q67] 设置隔离级别
来源：http://kbx.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qro.yuxming.cn

[Q68] 保存点
来源：http://sht.hnxiangtu.top

SAVEPOINT sp1;
来源：http://iwv.yueranfly.top

ROLLBACK TO sp1;
来源：http://tnf.9152youxi.cn

[Q69] 查看执行计划
来源：http://ovx.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hzk.zhengqikj.top

[Q70] 更新统计信息
来源：http://jxz.aizwys.cn

ANALYZE TABLE users;
来源：http://poj.jlsjyb.cn

[Q71] 查看建表语句
来源：http://dna.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oxw.yangfankeji.com

[Q72] 查看索引
来源：http://ctm.hysaishi.cn

SHOW INDEX FROM users;
来源：http://iwp.redwolf501.top

[Q73] 查看表状态
来源：http://bba.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ugg.hesvh.cn

[Q74] 强制使用索引
来源：http://suu.guowangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bef.yj202588.top

[Q75] 日期格式化
来源：http://erl.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dql.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xiq.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://tul.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mge.zdqjudy.top

[Q77] 时间加减
来源：http://fbc.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jar.yj202588.top

[Q78] 当前时间
来源：http://byd.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qzq.uphjek.com

[Q79] 字符串拼接
来源：http://zdk.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ynp.bjfxy.top

[Q80] 字符串截取
来源：http://hwf.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fii.ydjk.org.cn

[Q81] 字符串替换
来源：http://bdh.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cwy.shangyingyoupin.top

[Q82] 字符长度与字节长度
来源：http://egu.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qqi.vqdsnc.cn

[Q83] 大小写转换
来源：http://xbp.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pnc.ydzc1.top

[Q84] 去除首尾空格
来源：http://gng.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://ahc.hcnkem.com

[Q85] 数值取整
来源：http://yzc.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iwm.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://gmu.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kzs.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://deh.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lhc.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://sae.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xkp.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iqd.ehwqpu.com

[Q89] 判断表是否存在
来源：http://osw.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nok.zdbjq.cn

[Q90] 生成序号列
来源：http://ezv.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kqo.guowangkeji.top

================================================================================
来源：http://ahr.jinqigfzy.top

R. Bash 专题
来源：http://pyg.shanyushiyangtech.top

================================================================================
来源：http://tqb.gogol.net.cn

[R01] shebang 与严格模式
来源：http://inr.fzhhl.top

#!/usr/bin/env bash
来源：http://zyb.tianlin.xyz

set -euo pipefail
来源：http://ajx.tanke756.top

[R02] 变量赋值与使用
来源：http://vjw.fktsv.cn

name="Tom"; echo "$name"
来源：http://dkb.vqdsnc.cn

[R03] 只读变量
来源：http://rxo.xziqi.cn

readonly PI=3.14
来源：http://dbh.chenjidiqi.icu

[R04] 位置参数
来源：http://czj.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://shi.sweek.top

[R05] 参数默认值
来源：http://bjf.tanke756.top

name="${1:-default}"
来源：http://nlf.nanxuanxn.top

[R06] 判断命令是否存在
来源：http://bpg.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ppt.hfpthk.cn

[R07] if 判断文件
来源：http://dbr.yj202588.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://njf.52xcode.cn

[R08] 数值比较
来源：http://htp.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://drh.yj202588.top

[R09] 字符串比较
来源：http://bhz.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lph.yj20258888.top

[R10] 正则匹配
来源：http://upw.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ctc.cqqwz.cn

[R11] case 多分支
来源：http://ccc.ywan-chungtsiang.top

case "$1" in
来源：http://dnv.jinqigufen.top

start) echo "启动" ;;
来源：http://gww.zhengqikj.top

stop)  echo "停止" ;;
来源：http://uar.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://hsn.daria6918.cn

esac
来源：http://fjt.chenjidiqi.icu

[R12] for 遍历文件
来源：http://blw.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://zis.zhaomingkeji.xyz

[R13] for 计数循环
来源：http://ddc.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://ura.zdqjudy.top

[R14] C 风格 for
来源：http://ans.shanyushiyangtech.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aip.cqqwz.cn

[R15] while 逐行读文件
来源：http://fbg.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lse.yj20258888.top

[R16] until 等待条件
来源：http://gsf.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yib.gogol.net.cn

[R17] 数组定义与取值
来源：http://pjl.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://irm.cdnleiting.top

[R18] 遍历数组
来源：http://don.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bnt.zhoulong.xyz

[R19] 数组长度
来源：http://pgd.yangfankeji.com

echo "${#arr[@]}"
来源：http://yos.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://kka.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pgf.hnqzz.top

[R21] 字符串长度
来源：http://rzq.iojbl.cn

echo "${#s}"
来源：http://yfp.andypj.xyz

[R22] 截取子串
来源：http://qfw.tianlin.xyz

echo "${s:0:5}"
来源：http://ehy.zycfv.cn

[R23] 字符串替换
来源：http://wfx.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nae.jinqigufen.top

[R24] 大小写转换
来源：http://icn.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://cty.sysykeji.top

[R25] 去后缀 / 去前缀
来源：http://hox.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hlk.dianchejie.cn

[R26] 命令替换
来源：http://lvi.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://qig.jqgfzy.top

[R27] 算术展开
来源：http://cad.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://syf.svipenyu.cn

[R28] 浮点运算
来源：http://wwf.bjfxy.top

echo "scale=2; 10/3" | bc
来源：http://xgz.c1oappe.top

[R29] 定义函数
来源：http://bmn.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gid.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://cau.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://efk.nanxinkj.top

[R31] 局部变量
来源：http://hsa.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://lpc.pycfn.com

[R32] 参数个数校验
来源：http://rkj.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://igu.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://yvr.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lns.mhx1999.top

[R34] 退出时清理
来源：http://ptc.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://dsy.guannengcc.top

[R35] 后台执行并等待
来源：http://kky.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nlg.yueranfly.top

[R36] 并发执行多个任务
来源：http://ncc.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ysc.gzhubu.top

[R37] 把输出赋给变量
来源：http://fxb.gzhubu.top

files=$(ls -1)
来源：http://obd.aizwys.cn

[R38] 管道串联
来源：http://ath.ivvv.top

cat a.txt | grep -i error | wc -l
来源：http://dra.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://tzs.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://skl.zhongyouzk.top

[R40] 追加写日志
来源：http://xid.aibaodan.cn

echo "log" >> out.log
来源：http://ats.nwbrower.top

[R41] 丢弃输出
来源：http://ubh.zhiwuduotai.top

cmd >/dev/null 2>&1
来源：http://fvt.zhongyouzk.top

[R42] 输入重定向
来源：http://cax.shanyushiyangtech.top

wc -l < a.txt
来源：http://kpy.guannengcc.top

[R43] 按名字查找文件
来源：http://jpz.mhx1999.top

find . -name "*.log" -type f
来源：http://vvd.quarkkingdee.top

[R44] 按修改时间查找
来源：http://fvn.dashuyun.cn

find . -mtime -7 -type f
来源：http://ewu.jlsjyb.cn

[R45] 批量删除
来源：http://tbq.kuanghao11.cn

find . -name "*.tmp" -delete
来源：http://zxa.yfazqb.com

[R46] 递归替换文件内容
来源：http://tim.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jne.yuanzhike.top

[R47] sed 单行替换
来源：http://jbf.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://wzn.wangshuangyany.cn

[R48] awk 取指定列
来源：http://uwa.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://vpv.zycfv.cn

[R49] awk 带条件
来源：http://whf.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mwb.nanxinkj.top

[R50] awk 求和
来源：http://yzw.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://ksn.yueranfly.top

[R51] 排序去重取前几
来源：http://eqd.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hsj.gogol.net.cn

[R52] 统计行数
来源：http://ixv.yj20258.top

wc -l a.txt
来源：http://cul.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://mpx.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rau.hongshengwenyu.top

[R54] 比较两个文件
来源：http://yil.uphjek.com

diff a.txt b.txt
来源：http://ecr.bjfxy.top

[R55] 压缩与解压
来源：http://ayi.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uip.nwbrower.top

[R56] 远程拷贝
来源：http://ejj.birdmap.top

scp file user@host:/path/
来源：http://dnk.yvedp.cn

[R57] 远程执行命令
来源：http://ovs.xuanzx.com

ssh user@host 'uptime'
来源：http://mhu.mhx1999.top

[R58] 下载文件
来源：http://xxh.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fai.yj202588.top

[R59] 发 POST JSON
来源：http://uim.xylfe.cn


<!-- 参考信息 -->