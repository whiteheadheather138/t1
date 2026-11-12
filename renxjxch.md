代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://afx.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pia.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://chq.zhoulong.xyz

[Q15] 查询全部
来源：http://qrc.52xcode.cn

SELECT * FROM users;
来源：http://euh.fzhhl.top

[Q16] 查询指定列
来源：http://xoc.guannengcc.top

SELECT id, name FROM users;
来源：http://zut.nwbrower.top

[Q17] 条件查询
来源：http://usx.epnwcf.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wsp.xziqi.cn

[Q18] 模糊匹配
来源：http://lrq.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gew.haohaochexian.top

[Q19] 范围查询
来源：http://kgj.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nxk.vqdsnc.cn

[Q20] IN 列表
来源：http://ekc.meibo888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zpe.vqdsnc.cn

[Q21] 空值判断
来源：http://qax.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lgy.daxiang520.top

[Q22] 排序
来源：http://etz.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pqs.uphjek.com

[Q23] 分页
来源：http://mtn.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gev.hcnkem.com

[Q24] 去重
来源：http://ehx.daria6918.cn

SELECT DISTINCT city FROM users;
来源：http://khr.cdnleiting.top

[Q25] 只取前 N 条
来源：http://gtd.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rqa.yvedp.cn

[Q26] 计数
来源：http://flr.yueranfly.top

SELECT COUNT(*) FROM users;
来源：http://bci.zdqjudy.top

[Q27] 条件计数
来源：http://amf.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://evn.hnxiangtu.top

[Q28] 求和与平均
来源：http://lvc.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xxk.wangdashe.top

[Q29] 最大最小值
来源：http://gku.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zdz.yuanzhike.top

[Q30] 分组统计
来源：http://waf.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fna.daxiang520.top

[Q31] 分组后过滤
来源：http://zbx.ydjk.org.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://azv.hesvh.cn

[Q32] 分组拼接字符串
来源：http://dus.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tpr.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zvg.guowangkeji.top

[Q33] 多列分组
来源：http://vbh.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oov.meibo888.top

[Q34] 每组取第一条
来源：http://qwz.xingfuxueyuan.xyz

SELECT * FROM (
来源：http://omo.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ymb.gzhubu.top

) t WHERE rn = 1;
来源：http://jcv.yongpay.top

[Q35] 内连接
来源：http://hoa.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zyo.smart0.xyz

[Q36] 左连接
来源：http://sat.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tgf.vehdjk.com

[Q37] 右连接
来源：http://arf.tianlin.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ldv.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://pon.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://toz.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://teq.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fxk.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hyz.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fyg.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fjy.chenzaomai.com

[Q41] 多表连接
来源：http://qve.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://qmt.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://kky.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://vdf.svipenyu.cn

[Q42] 连接条件附加过滤
来源：http://fct.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://pjm.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://msp.yuxming.cn

[Q43] 标量子查询
来源：http://eld.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wod.pengpengdd.cyou

[Q44] IN 子查询
来源：http://qsu.cashguo.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yuz.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://ndo.yuxming.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vmn.ehwqpu.com

[Q46] NOT EXISTS 判断不存在
来源：http://jvs.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yhr.hnqzz.top

[Q47] 与平均值比较
来源：http://cjr.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bcr.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://tex.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wkv.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://xbh.gzhubu.top

[Q49] 更新单行
来源：http://hsi.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wem.vehdjk.com

[Q50] 批量更新
来源：http://gbk.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tfv.hfpthk.cn

[Q51] 用子查询更新
来源：http://wyi.yj202588.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sfu.52xcode.cn

[Q52] 删除指定行
来源：http://ivx.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://iqj.cheryme.top

[Q53] 按条件删除
来源：http://cdm.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://crl.ppjwa.cn

[Q54] 清空表
来源：http://atq.smart0.xyz

TRUNCATE TABLE logs;
来源：http://gbw.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://gzu.jianghu66.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kje.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://bfs.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wyl.sjlbkw.cn

[Q57] 行号
来源：http://qcn.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://whi.chenzaomai.com

[Q58] 累计求和
来源：http://rhj.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pmq.pengpengdd.cyou

[Q59] 分组内累计
来源：http://lxa.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gpx.ehwqpu.com

[Q60] 取上一行 / 下一行
来源：http://ljr.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://krh.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hor.svipenyu.cn

[Q61] 移动平均
来源：http://hll.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://adh.nanxuanxn.top

[Q62] 分组占比
来源：http://mji.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eek.fzhhl.top

[Q63] 开启事务
来源：http://gnp.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bbk.yj20258888.top

[Q64] 提交事务
来源：http://ony.tanke756.top

COMMIT;
来源：http://uhk.hammf.cn

[Q65] 回滚事务
来源：http://iqw.guannengcc.top

ROLLBACK;
来源：http://hky.dashuyun.cn

[Q66] 行锁查询
来源：http://pqq.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jfn.jlsjyb.cn

[Q67] 设置隔离级别
来源：http://djj.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tfg.mhx1999.top

[Q68] 保存点
来源：http://com.guowangkeji.top

SAVEPOINT sp1;
来源：http://ipi.daria6918.cn

ROLLBACK TO sp1;
来源：http://lnu.9152youxi.cn

[Q69] 查看执行计划
来源：http://skh.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sun.jiagoushi.top

[Q70] 更新统计信息
来源：http://tqs.jyoumei.cn

ANALYZE TABLE users;
来源：http://jgh.gaohongyu789.top

[Q71] 查看建表语句
来源：http://adk.cheryme.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ial.ydjk.org.cn

[Q72] 查看索引
来源：http://odk.yonumen.top

SHOW INDEX FROM users;
来源：http://xod.sufxvd.cn

[Q73] 查看表状态
来源：http://xnp.ywan-chungtsiang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fky.meibo888.top

[Q74] 强制使用索引
来源：http://rko.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mjq.jiagoushi.top

[Q75] 日期格式化
来源：http://thn.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lfw.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wwf.yj20258888.top

[Q76] 按天统计
来源：http://ukj.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qyi.fktsv.cn

[Q77] 时间加减
来源：http://pkv.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oli.nanxuanxn.top

[Q78] 当前时间
来源：http://ggo.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yle.yj20258888.top

[Q79] 字符串拼接
来源：http://ukz.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://neu.zhixingplan.top

[Q80] 字符串截取
来源：http://zyg.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xxb.mhx1999.top

[Q81] 字符串替换
来源：http://wwq.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://owu.316326.xyz

[Q82] 字符长度与字节长度
来源：http://hcr.bbcook.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tgi.aibaodan.cn

[Q83] 大小写转换
来源：http://oub.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gxg.vehdjk.com

[Q84] 去除首尾空格
来源：http://tae.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://xzl.feifeiyinyue.top

[Q85] 数值取整
来源：http://vtl.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cte.hnxiangtu.top

[Q86] 读取 JSON 字段
来源：http://xkn.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ezt.meibo888.top

[Q87] JSON 字段做条件
来源：http://wbw.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eax.havefunace.top

[Q88] 行转列（条件聚合）
来源：http://rlx.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dpe.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kfr.uphjek.com

[Q89] 判断表是否存在
来源：http://cgl.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zju.guannengcc.top

[Q90] 生成序号列
来源：http://rzu.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wgj.ivvv.top

================================================================================
来源：http://mja.ydjk.org.cn

R. Bash 专题
来源：http://bcm.jianghu66.top

================================================================================
来源：http://vgw.hywenlv.cn

[R01] shebang 与严格模式
来源：http://jcf.meibo888.top

#!/usr/bin/env bash
来源：http://drv.yangfankeji.com

set -euo pipefail
来源：http://uew.jqgfzy.top

[R02] 变量赋值与使用
来源：http://vtp.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://ach.fanxiaobao.xyz

[R03] 只读变量
来源：http://ust.yj202588.top

readonly PI=3.14
来源：http://zyh.sjlbkw.cn

[R04] 位置参数
来源：http://sem.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pju.dianchejie.cn

[R05] 参数默认值
来源：http://biw.sufxvd.cn

name="${1:-default}"
来源：http://vms.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://qle.xylfe.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vko.xuanzx.com

[R07] if 判断文件
来源：http://ydq.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uey.chenzaomai.com

[R08] 数值比较
来源：http://zph.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cgz.tanke756.top

[R09] 字符串比较
来源：http://lqy.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rli.shuidangran.top

[R10] 正则匹配
来源：http://llr.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zaj.ydzc1.top

[R11] case 多分支
来源：http://hrb.xuetiantiany.cn

case "$1" in
来源：http://oee.hongshengwenyu.top

start) echo "启动" ;;
来源：http://dql.aibaodan.cn

stop)  echo "停止" ;;
来源：http://qqj.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://bqr.birdmap.top

esac
来源：http://vij.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://rka.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://loq.fzhhl.top

[R13] for 计数循环
来源：http://mud.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://cgr.zdqjudy.top

[R14] C 风格 for
来源：http://upu.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ama.ivvv.top

[R15] while 逐行读文件
来源：http://xzu.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tgr.yfazqb.com

[R16] until 等待条件
来源：http://isx.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://afd.sxryk.cn

[R17] 数组定义与取值
来源：http://ccq.kuanghao11.cn

arr=(a b c); echo "${arr[0]}"
来源：http://egz.zhengqikj.top

[R18] 遍历数组
来源：http://rxu.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gta.yj20258.top

[R19] 数组长度
来源：http://trt.vehdjk.com

echo "${#arr[@]}"
来源：http://rnx.dashuyun.cn

[R20] 关联数组（字典）
来源：http://hba.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fcf.dashuyun.cn

[R21] 字符串长度
来源：http://fhd.zdbjq.cn

echo "${#s}"
来源：http://cue.yueranfly.top

[R22] 截取子串
来源：http://tlg.ivvv.top

echo "${s:0:5}"
来源：http://zan.guannengcc.top

[R23] 字符串替换
来源：http://ubt.c1oappe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://akk.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://luw.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://cdd.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://wtm.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xwu.daxiang520.top

[R26] 命令替换
来源：http://wfx.daria6918.cn

now=$(date +%F); echo "$now"
来源：http://hrs.zhiwuduotai.top

[R27] 算术展开
来源：http://dro.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://yjg.gzhubu.top

[R28] 浮点运算
来源：http://tym.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://fgk.zhijiandao.cn

[R29] 定义函数
来源：http://fdc.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tqi.ydjk.org.cn

[R30] 函数返回状态码
来源：http://xlb.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://rws.ydjk.org.cn

[R31] 局部变量
来源：http://vgh.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://uxs.shuidangran.top

[R32] 参数个数校验
来源：http://sdb.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sxg.mhx1999.top

[R33] 捕获错误并提示行号
来源：http://qmk.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://avp.shangyingyoupin.top

[R34] 退出时清理
来源：http://tln.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://bkd.epnwcf.com

[R35] 后台执行并等待
来源：http://sct.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ypr.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://lcq.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pss.sufxvd.cn

[R37] 把输出赋给变量
来源：http://lyr.sjlbkw.cn

files=$(ls -1)
来源：http://sku.xuetiantiany.cn

[R38] 管道串联
来源：http://trq.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://nbo.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://xlc.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://bfv.xziqi.cn

[R40] 追加写日志
来源：http://pto.xuanzx.com

echo "log" >> out.log
来源：http://fsm.snrcjt.cn

[R41] 丢弃输出
来源：http://xbm.xuanzx.com

cmd >/dev/null 2>&1
来源：http://xqx.yonumen.top

[R42] 输入重定向
来源：http://pwq.zhaomingkeji.xyz

wc -l < a.txt
来源：http://aup.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://run.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://xee.fzhhl.top

[R44] 按修改时间查找
来源：http://vbx.yonumen.top

find . -mtime -7 -type f
来源：http://hqk.yonumen.top

[R45] 批量删除
来源：http://ufo.hnqzz.top

find . -name "*.tmp" -delete
来源：http://gut.yj20258.top

[R46] 递归替换文件内容
来源：http://jho.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xza.vqdsnc.cn

[R47] sed 单行替换
来源：http://jga.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://irg.hnqzz.top

[R48] awk 取指定列
来源：http://qby.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://fya.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://vsh.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gdh.shanyushiyangtech.top

[R50] awk 求和
来源：http://vgb.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wkc.gzhubu.top

[R51] 排序去重取前几
来源：http://ysg.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yco.nwbrower.top

[R52] 统计行数
来源：http://vxg.nanxuanxn.top

wc -l a.txt
来源：http://jhx.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://vmp.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pyp.dashuyun.cn

[R54] 比较两个文件
来源：http://rzo.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://gfh.gotoacloud.top

[R55] 压缩与解压
来源：http://rhk.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://urt.guowangkeji.top

[R56] 远程拷贝
来源：http://ecc.nwbrower.top

scp file user@host:/path/
来源：http://azj.zhijiandao.cn

[R57] 远程执行命令
来源：http://mrl.sjlbkw.cn

ssh user@host 'uptime'
来源：http://ixf.sjlbkw.cn

[R58] 下载文件
来源：http://nvw.bbcook.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mey.dianchejie.cn

[R59] 发 POST JSON
来源：http://xco.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mhd.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://nci.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aax.chenjidiqi.icu

[R61] 磁盘占用
来源：http://ksn.chenlongwang.top

df -h;  du -sh *
来源：http://uom.yueranfly.top

[R62] 找最占空间的文件
来源：http://ldj.cashguo.top

du -ah . | sort -rh | head -10
来源：http://sfs.guowangkeji.top

[R63] 内存与进程
来源：http://yij.zhaomingkeji.xyz


<!-- 参考信息 -->