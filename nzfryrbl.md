代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://glh.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oau.cashguo.top

[Q13] 忽略重复插入
来源：http://ixj.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vld.gotoacloud.top

[Q14] 存在则更新（upsert）
来源：http://kqh.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vaj.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bpm.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://ibo.cqqwz.cn

SELECT * FROM users;
来源：http://yqf.hfpthk.cn

[Q16] 查询指定列
来源：http://jmu.0kj1m.cn

SELECT id, name FROM users;
来源：http://equ.fktsv.cn

[Q17] 条件查询
来源：http://foy.yuxming.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hrc.cucudq.cn

[Q18] 模糊匹配
来源：http://gyp.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://acp.havefunace.top

[Q19] 范围查询
来源：http://idj.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pfv.epnwcf.com

[Q20] IN 列表
来源：http://qan.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kdx.jianghu66.top

[Q21] 空值判断
来源：http://ekp.zdbjq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fpc.zhiwuduotai.top

[Q22] 排序
来源：http://bqs.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gwp.jqgufenzy.top

[Q23] 分页
来源：http://yoz.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cgs.quarkkingdee.top

[Q24] 去重
来源：http://rtd.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://ojx.zdqjudy.top

[Q25] 只取前 N 条
来源：http://pvs.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bhs.jianghu66.top

[Q26] 计数
来源：http://ugn.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://rmv.hcnkem.com

[Q27] 条件计数
来源：http://lny.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dch.haohaochexian.top

[Q28] 求和与平均
来源：http://wod.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pah.yanxiufei.cn

[Q29] 最大最小值
来源：http://zfo.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://baf.jyoumei.cn

[Q30] 分组统计
来源：http://xpb.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rgy.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://lus.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jiq.xziqi.cn

[Q32] 分组拼接字符串
来源：http://ttf.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ilg.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pcm.fanxiaobao.xyz

[Q33] 多列分组
来源：http://qhs.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xvz.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://fpo.fanxiaobao.xyz

SELECT * FROM (
来源：http://ndk.xingfuxueyuan.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tto.guannengcc.top

) t WHERE rn = 1;
来源：http://otr.havefunace.top

[Q35] 内连接
来源：http://orc.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vcu.ppjwa.cn

[Q36] 左连接
来源：http://tfu.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lzy.shanyushiyangtech.top

[Q37] 右连接
来源：http://qhm.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ysw.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://qoh.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bfa.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://ufw.sxryk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jvp.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yex.sysykeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rxb.fzhhl.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://msw.pengpengdd.cyou

[Q41] 多表连接
来源：http://cmn.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mub.ybcxt.top

JOIN users u ON u.id = o.user_id
来源：http://vep.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://sot.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://dpf.zhoulong.xyz

SELECT u.name, o.amount FROM users u
来源：http://kwp.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wur.redwolf501.top

[Q43] 标量子查询
来源：http://faf.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://abi.tianlin.xyz

[Q44] IN 子查询
来源：http://swi.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hch.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://onb.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dwh.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://aos.tian-w.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bsd.fengsongda.top

[Q47] 与平均值比较
来源：http://fxm.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qmo.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://zwi.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cin.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://tbz.gzhubu.top

[Q49] 更新单行
来源：http://hhx.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vfk.vehdjk.com

[Q50] 批量更新
来源：http://wxz.hesvh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ypv.yueranfly.top

[Q51] 用子查询更新
来源：http://kad.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wcm.daxiang520.top

[Q52] 删除指定行
来源：http://xek.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://omx.fehbvm.com

[Q53] 按条件删除
来源：http://lcz.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yjx.jiagoushi.top

[Q54] 清空表
来源：http://png.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://kkj.daria6918.cn

[Q55] 排名（并列占位）
来源：http://sqe.birdmap.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zjx.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://vgk.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lng.ivvv.top

[Q57] 行号
来源：http://szt.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kvl.iojbl.cn

[Q58] 累计求和
来源：http://pjd.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uax.jyoumei.cn

[Q59] 分组内累计
来源：http://qfh.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bvw.shangyingyoupin.top

[Q60] 取上一行 / 下一行
来源：http://rrn.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://upm.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://afg.havefunace.top

[Q61] 移动平均
来源：http://rzn.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://osz.sufxvd.cn

[Q62] 分组占比
来源：http://osb.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dno.zhaomingkeji.xyz

[Q63] 开启事务
来源：http://ioj.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rkh.ydzc1.top

[Q64] 提交事务
来源：http://dht.jlsjyb.cn

COMMIT;
来源：http://zbb.mhx1999.top

[Q65] 回滚事务
来源：http://kgg.svipenyu.cn

ROLLBACK;
来源：http://pvy.yj20258888.top

[Q66] 行锁查询
来源：http://mwk.fktsv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bco.haohaochexian.top

[Q67] 设置隔离级别
来源：http://vjl.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zqe.feifeiyinyue.top

[Q68] 保存点
来源：http://lcn.jqgufenzy.top

SAVEPOINT sp1;
来源：http://kso.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://fbj.jinqigufen.top

[Q69] 查看执行计划
来源：http://xkp.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ksd.wangdashe.top

[Q70] 更新统计信息
来源：http://mqw.xinyue.icu

ANALYZE TABLE users;
来源：http://ivg.tianlin.xyz

[Q71] 查看建表语句
来源：http://xmh.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eli.ppjwa.cn

[Q72] 查看索引
来源：http://aps.xuanzx.com

SHOW INDEX FROM users;
来源：http://xok.hfpthk.cn

[Q73] 查看表状态
来源：http://vma.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://azm.fktsv.cn

[Q74] 强制使用索引
来源：http://bko.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://htu.birdmap.top

[Q75] 日期格式化
来源：http://fqc.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://orf.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mrl.ydjk.org.cn

[Q76] 按天统计
来源：http://vrk.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oqe.shangyingyoupin.top

[Q77] 时间加减
来源：http://skn.yueranfly.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://znn.pengpengdd.cyou

[Q78] 当前时间
来源：http://ars.yvedp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ppa.xziqi.cn

[Q79] 字符串拼接
来源：http://pqv.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mxd.jqgfzy.top

[Q80] 字符串截取
来源：http://dzz.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qmn.hammf.cn

[Q81] 字符串替换
来源：http://isi.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ixz.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://cax.chenjidiqi.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yyk.snrcjt.cn

[Q83] 大小写转换
来源：http://vfq.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tcw.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://srh.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://cip.sufxvd.cn

[Q85] 数值取整
来源：http://jhv.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tkj.meibo888.top

[Q86] 读取 JSON 字段
来源：http://ljn.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aqq.shuidangran.top

[Q87] JSON 字段做条件
来源：http://ggr.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wmx.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://wfb.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mbf.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ovt.yonumen.top

[Q89] 判断表是否存在
来源：http://fgb.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dch.ppjwa.cn

[Q90] 生成序号列
来源：http://uso.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vyr.hysaishi.cn

================================================================================
来源：http://rft.xziqi.cn

R. Bash 专题
来源：http://cyg.0kj1m.cn

================================================================================
来源：http://bch.hfpthk.cn

[R01] shebang 与严格模式
来源：http://yqn.dianchejie.cn

#!/usr/bin/env bash
来源：http://fzp.tianlin.xyz

set -euo pipefail
来源：http://bmc.guowangkeji.top

[R02] 变量赋值与使用
来源：http://dqj.jinyuanbaomall.cn

name="Tom"; echo "$name"
来源：http://xqb.hcnkem.com

[R03] 只读变量
来源：http://odg.jinyuanbaomall.cn

readonly PI=3.14
来源：http://lfo.daria6918.cn

[R04] 位置参数
来源：http://hab.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ahh.c1oappe.top

[R05] 参数默认值
来源：http://amw.jinyuanbaomall.cn

name="${1:-default}"
来源：http://irq.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://wau.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zvl.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://qhz.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://otx.shzxlz.cn

[R08] 数值比较
来源：http://izv.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mas.jinqigufen.top

[R09] 字符串比较
来源：http://cal.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nps.jinghuilouyu.cn

[R10] 正则匹配
来源：http://riu.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vtv.zhoulong.xyz

[R11] case 多分支
来源：http://phd.birdmap.top

case "$1" in
来源：http://xtw.dianchejie.cn

start) echo "启动" ;;
来源：http://xdt.dianchejie.cn

stop)  echo "停止" ;;
来源：http://ove.ybcxt.top

*)     echo "未知命令" ;;
来源：http://iri.shanyushiyangkeji.top

esac
来源：http://jez.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://hwj.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://zij.xuetiantiany.cn

[R13] for 计数循环
来源：http://ybr.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://ctc.hysaishi.cn

[R14] C 风格 for
来源：http://qtq.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ium.xziqi.cn

[R15] while 逐行读文件
来源：http://kpr.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://myl.uphjek.com

[R16] until 等待条件
来源：http://oeo.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fpp.9152youxi.cn

[R17] 数组定义与取值
来源：http://usv.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://rik.yonumen.top

[R18] 遍历数组
来源：http://teu.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qcn.redwolf501.top

[R19] 数组长度
来源：http://gbv.hcnkem.com

echo "${#arr[@]}"
来源：http://evy.cqqwz.cn

[R20] 关联数组（字典）
来源：http://oem.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gmt.andypj.xyz

[R21] 字符串长度
来源：http://jvg.iojbl.cn

echo "${#s}"
来源：http://tvd.fehbvm.com

[R22] 截取子串
来源：http://mfl.xziqi.cn

echo "${s:0:5}"
来源：http://odx.ctjpmb.com

[R23] 字符串替换
来源：http://olo.shanyushiyangtech.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ktr.yueranfly.top

[R24] 大小写转换
来源：http://ewy.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://oax.ydjk.org.cn

[R25] 去后缀 / 去前缀
来源：http://eiz.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ebl.jlsjyb.cn

[R26] 命令替换
来源：http://lpe.cdnleiting.top

now=$(date +%F); echo "$now"
来源：http://tyf.ppjwa.cn

[R27] 算术展开
来源：http://sfy.yonumen.top

echo $((1 + 2 * 3))
来源：http://qzu.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://neh.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://htp.yueranfly.top

[R29] 定义函数
来源：http://mhl.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wae.fktsv.cn

[R30] 函数返回状态码
来源：http://blf.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://yhg.vqdsnc.cn

[R31] 局部变量
来源：http://fwr.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://xmg.yuanzhike.top

[R32] 参数个数校验
来源：http://mbe.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jtp.cashguo.top

[R33] 捕获错误并提示行号
来源：http://wjf.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qjr.yonumen.top

[R34] 退出时清理
来源：http://vqp.xylfe.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fpr.sweek.top

[R35] 后台执行并等待
来源：http://owj.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kvk.chenlongwang.top

[R36] 并发执行多个任务
来源：http://rfn.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jsa.dianchejie.cn

[R37] 把输出赋给变量
来源：http://shs.xuanzx.com

files=$(ls -1)
来源：http://cvc.xuanzx.com

[R38] 管道串联
来源：http://eym.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://gws.havefunace.top

[R39] 重定向标准输出与错误
来源：http://cmi.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://mkr.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://skn.hnqzz.top

echo "log" >> out.log
来源：http://spr.cdnleiting.top

[R41] 丢弃输出
来源：http://yxv.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://dpz.c1oappe.top

[R42] 输入重定向
来源：http://gzr.shangyingyoupin.top

wc -l < a.txt
来源：http://gtk.yj20258.top

[R43] 按名字查找文件
来源：http://jol.ybcxt.top

find . -name "*.log" -type f
来源：http://dml.guowangkeji.top

[R44] 按修改时间查找
来源：http://vpj.xuanzx.com

find . -mtime -7 -type f
来源：http://owo.chenzaomai.com

[R45] 批量删除
来源：http://pgp.hysaishi.cn

find . -name "*.tmp" -delete
来源：http://rgq.uphjek.com

[R46] 递归替换文件内容
来源：http://qht.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zyu.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://cfp.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://ils.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://lzb.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://lzj.fktsv.cn

[R49] awk 带条件
来源：http://rzx.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://odh.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://ysu.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://ibj.jlsjyb.cn

[R51] 排序去重取前几
来源：http://ors.fengsongda.top

sort a.txt | uniq -c | sort -rn | head
来源：http://avg.ehwqpu.com

[R52] 统计行数
来源：http://eza.yongpay.top

wc -l a.txt
来源：http://trx.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://bwv.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ycu.ehwqpu.com

[R54] 比较两个文件
来源：http://ncf.shzxlz.cn

diff a.txt b.txt
来源：http://cko.gaohongyu789.top

[R55] 压缩与解压
来源：http://bkx.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dln.vqdsnc.cn

[R56] 远程拷贝
来源：http://suh.mhx1999.top

scp file user@host:/path/
来源：http://fzj.gotoacloud.top

[R57] 远程执行命令
来源：http://tst.xuanzx.com

ssh user@host 'uptime'
来源：http://qke.snrcjt.cn

[R58] 下载文件
来源：http://jtl.bbcook.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pzg.bbcook.cn

[R59] 发 POST JSON
来源：http://cpj.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sqx.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://cjc.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oai.fehbvm.com

[R61] 磁盘占用
来源：http://bzz.uphjek.com


<!-- 参考信息 -->