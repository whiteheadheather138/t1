代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://qih.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gjp.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ilz.dashuyun.cn

[Q15] 查询全部
来源：http://tme.vqdsnc.cn

SELECT * FROM users;
来源：http://axq.hammf.cn

[Q16] 查询指定列
来源：http://cfx.daria6918.cn

SELECT id, name FROM users;
来源：http://egk.nanxuanxn.top

[Q17] 条件查询
来源：http://rqi.ppjwa.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mav.c1oappe.top

[Q18] 模糊匹配
来源：http://hww.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://owp.ydzc1.top

[Q19] 范围查询
来源：http://ywf.chenlongwang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://krk.sxryk.cn

[Q20] IN 列表
来源：http://tfx.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xgc.dianchejie.cn

[Q21] 空值判断
来源：http://rdt.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hug.sysykeji.top

[Q22] 排序
来源：http://orv.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aiz.tian-w.cn

[Q23] 分页
来源：http://trs.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jzt.epnwcf.com

[Q24] 去重
来源：http://zgx.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://hfp.shuidangran.top

[Q25] 只取前 N 条
来源：http://ubc.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dbq.zdbjq.cn

[Q26] 计数
来源：http://otf.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://phh.birdmap.top

[Q27] 条件计数
来源：http://dwt.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vyk.birdmap.top

[Q28] 求和与平均
来源：http://mug.jlsjyb.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wye.zhixingplan.top

[Q29] 最大最小值
来源：http://jnm.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cao.shanyushiyangtech.top

[Q30] 分组统计
来源：http://inx.jinqigfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gpq.0kj1m.cn

[Q31] 分组后过滤
来源：http://fdv.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bzs.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://qhw.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hwn.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ekv.yonumen.top

[Q33] 多列分组
来源：http://rvr.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mlm.hysaishi.cn

[Q34] 每组取第一条
来源：http://jvr.ehwqpu.com

SELECT * FROM (
来源：http://nss.jlsjyb.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://efv.quarkkingdee.top

) t WHERE rn = 1;
来源：http://ydz.jqgufenzy.top

[Q35] 内连接
来源：http://rzs.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lfb.xuanzx.com

[Q36] 左连接
来源：http://zrj.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bjv.ppjwa.cn

[Q37] 右连接
来源：http://bff.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://efn.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://tpp.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://few.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://jmr.316326.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://eul.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bla.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uqs.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ics.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://ffu.dianchejie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yzh.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://stw.xziqi.cn

JOIN products p ON p.id = o.product_id;
来源：http://dlf.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://zrq.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://voa.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rkf.jianghu66.top

[Q43] 标量子查询
来源：http://tsa.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sxl.daxiang520.top

[Q44] IN 子查询
来源：http://efy.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://syr.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://cmk.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dgk.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://eem.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://peq.chenlongwang.top

[Q47] 与平均值比较
来源：http://qzt.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nwf.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://bwy.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ysc.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://vgs.fktsv.cn

[Q49] 更新单行
来源：http://mvs.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jyb.mhx1999.top

[Q50] 批量更新
来源：http://zfh.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wep.fzhhl.top

[Q51] 用子查询更新
来源：http://lml.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gzp.ydzc1.top

[Q52] 删除指定行
来源：http://tsp.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://dix.wangshuangyany.cn

[Q53] 按条件删除
来源：http://eok.jlsjyb.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mat.jqgufenzy.top

[Q54] 清空表
来源：http://rcz.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://kwu.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://xzx.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tjk.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://xuz.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ykn.xuetiantiany.cn

[Q57] 行号
来源：http://wev.jqgfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kni.kuanghao11.cn

[Q58] 累计求和
来源：http://ych.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sbd.bbcook.cn

[Q59] 分组内累计
来源：http://ymt.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://evr.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://ynf.zhiwuduotai.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ywd.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mqk.zdbjq.cn

[Q61] 移动平均
来源：http://rfg.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jxq.nanxuanxn.top

[Q62] 分组占比
来源：http://sdo.yj202588.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://meg.xuetiantiany.cn

[Q63] 开启事务
来源：http://jlq.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://cfy.yfazqb.com

[Q64] 提交事务
来源：http://hep.tarul.cn

COMMIT;
来源：http://jmo.daxiang520.top

[Q65] 回滚事务
来源：http://src.yuxming.cn

ROLLBACK;
来源：http://uck.ppjwa.cn

[Q66] 行锁查询
来源：http://phw.yvedp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jls.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://vej.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aft.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://kga.ybcxt.top

SAVEPOINT sp1;
来源：http://byl.ybcxt.top

ROLLBACK TO sp1;
来源：http://srh.mhx1999.top

[Q69] 查看执行计划
来源：http://nxd.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bqk.gzhubu.top

[Q70] 更新统计信息
来源：http://mee.aibaodan.cn

ANALYZE TABLE users;
来源：http://tcj.hywenlv.cn

[Q71] 查看建表语句
来源：http://ffr.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aqa.shzxlz.cn

[Q72] 查看索引
来源：http://wry.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://idg.aizwys.cn

[Q73] 查看表状态
来源：http://igl.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bug.tianlin.xyz

[Q74] 强制使用索引
来源：http://iqc.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bfz.ppjwa.cn

[Q75] 日期格式化
来源：http://cfg.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wat.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://akl.fengsongda.top

[Q76] 按天统计
来源：http://ied.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://upt.dianchejie.cn

[Q77] 时间加减
来源：http://opv.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xlc.zycfv.cn

[Q78] 当前时间
来源：http://peh.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fbk.ehwqpu.com

[Q79] 字符串拼接
来源：http://woo.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sxt.xinyue.icu

[Q80] 字符串截取
来源：http://ksi.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fjw.tanke756.top

[Q81] 字符串替换
来源：http://pfu.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zsl.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://qsc.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zbf.jqgfzy.top

[Q83] 大小写转换
来源：http://rwo.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ixm.yj20258888.top

[Q84] 去除首尾空格
来源：http://jph.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://xdy.zhengqikj.top

[Q85] 数值取整
来源：http://jfs.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pmi.jyoumei.cn

[Q86] 读取 JSON 字段
来源：http://syj.hesvh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zds.sysykeji.top

[Q87] JSON 字段做条件
来源：http://bnk.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://orj.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://bbv.hywenlv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uzt.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zty.zdbjq.cn

[Q89] 判断表是否存在
来源：http://nlq.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://umo.dianchejie.cn

[Q90] 生成序号列
来源：http://mgj.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mbt.zhoulong.xyz

================================================================================
来源：http://rle.gaohongyu789.top

R. Bash 专题
来源：http://wtl.vehdjk.com

================================================================================
来源：http://zko.yfazqb.com

[R01] shebang 与严格模式
来源：http://vni.jyoumei.cn

#!/usr/bin/env bash
来源：http://grr.aizwys.cn

set -euo pipefail
来源：http://ort.xuanzx.com

[R02] 变量赋值与使用
来源：http://fzq.cqqwz.cn

name="Tom"; echo "$name"
来源：http://axu.shzxlz.cn

[R03] 只读变量
来源：http://ajs.ivvv.top

readonly PI=3.14
来源：http://wnf.jinqigfzy.top

[R04] 位置参数
来源：http://ueb.jianghu66.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ddt.epnwcf.com

[R05] 参数默认值
来源：http://xwz.ydjk.org.cn

name="${1:-default}"
来源：http://qkr.cqqwz.cn

[R06] 判断命令是否存在
来源：http://eme.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wxh.shangyingyoupin.top

[R07] if 判断文件
来源：http://otr.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rkz.xinyue.icu

[R08] 数值比较
来源：http://uew.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://aqx.9152youxi.cn

[R09] 字符串比较
来源：http://wsv.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yoi.yvedp.cn

[R10] 正则匹配
来源：http://kbd.sjlbkw.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nfj.daxiang520.top

[R11] case 多分支
来源：http://aoa.zhaomingkeji.xyz

case "$1" in
来源：http://aqf.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://ljo.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://hlm.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://vsw.9152youxi.cn

esac
来源：http://idp.hongshengwenyu.top

[R12] for 遍历文件
来源：http://jfp.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://sdl.feifeiyinyue.top

[R13] for 计数循环
来源：http://ngq.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://isj.316326.xyz

[R14] C 风格 for
来源：http://snt.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xdp.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://oua.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mul.cheryme.top

[R16] until 等待条件
来源：http://xuw.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xno.fktsv.cn

[R17] 数组定义与取值
来源：http://fsa.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wuk.yongpay.top

[R18] 遍历数组
来源：http://gfv.sufxvd.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://czf.jlsjyb.cn

[R19] 数组长度
来源：http://chx.yonumen.top

echo "${#arr[@]}"
来源：http://pkl.wangdashe.top

[R20] 关联数组（字典）
来源：http://lga.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gau.ydjk.org.cn

[R21] 字符串长度
来源：http://ldu.jlsjyb.cn

echo "${#s}"
来源：http://shl.redwolf501.top

[R22] 截取子串
来源：http://snm.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://mwx.zhengqikj.top

[R23] 字符串替换
来源：http://iif.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jpz.jqgfzy.top

[R24] 大小写转换
来源：http://tjq.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://peb.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://guh.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://kzd.birdmap.top

[R26] 命令替换
来源：http://xbt.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://xlx.52xcode.cn

[R27] 算术展开
来源：http://sqa.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://ujk.vehdjk.com

[R28] 浮点运算
来源：http://wlo.xinyue.icu

echo "scale=2; 10/3" | bc
来源：http://ioh.cqqwz.cn

[R29] 定义函数
来源：http://rmx.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://clp.yfazqb.com

[R30] 函数返回状态码
来源：http://usn.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://fge.feifeiyinyue.top

[R31] 局部变量
来源：http://ccw.yfazqb.com

f() { local x=1; echo "$x"; }
来源：http://ayk.mhx1999.top

[R32] 参数个数校验
来源：http://rtw.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tgm.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://xkk.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mpi.zhijiandao.cn

[R34] 退出时清理
来源：http://ukj.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://msf.yanxiufei.cn

[R35] 后台执行并等待
来源：http://pml.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vtu.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://llt.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jjh.fehbvm.com

[R37] 把输出赋给变量
来源：http://aga.shanyushiyangtech.top

files=$(ls -1)
来源：http://kvs.shuidangran.top

[R38] 管道串联
来源：http://utq.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://edx.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://tbg.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://xnq.yueranfly.top

[R40] 追加写日志
来源：http://jid.feifeiyinyue.top

echo "log" >> out.log
来源：http://tag.tianlin.xyz

[R41] 丢弃输出
来源：http://cze.yueranfly.top

cmd >/dev/null 2>&1
来源：http://awb.jqgufenzy.top

[R42] 输入重定向
来源：http://dli.shanyushiyangkeji.top

wc -l < a.txt
来源：http://wjt.shangyingyoupin.top

[R43] 按名字查找文件
来源：http://jtu.yangfankeji.com

find . -name "*.log" -type f
来源：http://fqh.dashuyun.cn

[R44] 按修改时间查找
来源：http://vjg.hcnkem.com

find . -mtime -7 -type f
来源：http://qbl.zhaomingkeji.xyz

[R45] 批量删除
来源：http://xfa.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://vzj.sufxvd.cn

[R46] 递归替换文件内容
来源：http://gbu.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gtg.sweek.top

[R47] sed 单行替换
来源：http://agz.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://fvh.jinqigufen.top

[R48] awk 取指定列
来源：http://zwq.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://nfl.havefunace.top

[R49] awk 带条件
来源：http://sdd.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lnh.bbcook.cn

[R50] awk 求和
来源：http://sps.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fek.yfazqb.com

[R51] 排序去重取前几
来源：http://bva.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hqm.fanxiaobao.xyz

[R52] 统计行数
来源：http://jpv.ybcxt.top

wc -l a.txt
来源：http://aek.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://zqc.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zos.jqgufenzy.top

[R54] 比较两个文件
来源：http://myh.hcnkem.com

diff a.txt b.txt
来源：http://qke.gzhubu.top

[R55] 压缩与解压
来源：http://uwd.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rza.wangshuangyany.cn

[R56] 远程拷贝
来源：http://bhd.tianlin.xyz

scp file user@host:/path/
来源：http://rmk.fengsongda.top

[R57] 远程执行命令
来源：http://kyp.hesvh.cn

ssh user@host 'uptime'
来源：http://dbm.shangyingyoupin.top

[R58] 下载文件
来源：http://wbm.tanke756.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ijz.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://gxv.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ule.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://mec.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eba.havefunace.top

[R61] 磁盘占用
来源：http://ykn.quarkkingdee.top

df -h;  du -sh *
来源：http://hxd.jianghu66.top

[R62] 找最占空间的文件
来源：http://jfz.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://yse.zhiwuduotai.top

[R63] 内存与进程
来源：http://boz.316326.xyz


<!-- 参考信息 -->