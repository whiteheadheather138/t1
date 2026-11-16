代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hlc.shanyushiyangtech.top

[Q18] 模糊匹配
来源：http://cxx.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xry.hammf.cn

[Q19] 范围查询
来源：http://ctg.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ujb.xinyue.icu

[Q20] IN 列表
来源：http://qwe.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hva.hesvh.cn

[Q21] 空值判断
来源：http://hyb.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aai.ehwqpu.com

[Q22] 排序
来源：http://gcn.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://azk.kuanghao11.cn

[Q23] 分页
来源：http://kek.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pmo.vqdsnc.cn

[Q24] 去重
来源：http://tcz.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://uuo.hywenlv.cn

[Q25] 只取前 N 条
来源：http://xis.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vbf.dianchejie.cn

[Q26] 计数
来源：http://zmq.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://vyj.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://vki.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gnx.birdmap.top

[Q28] 求和与平均
来源：http://vev.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ywo.shangyingyoupin.top

[Q29] 最大最小值
来源：http://dpn.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hrh.hongshengwenyu.top

[Q30] 分组统计
来源：http://csg.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xfn.sjlbkw.cn

[Q31] 分组后过滤
来源：http://wxy.daria6918.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://khh.smart0.xyz

[Q32] 分组拼接字符串
来源：http://leo.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://efn.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zjm.yj20258888.top

[Q33] 多列分组
来源：http://iih.zhiwuduotai.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rkp.ybcxt.top

[Q34] 每组取第一条
来源：http://nbt.sjlbkw.cn

SELECT * FROM (
来源：http://pgj.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fbb.sweek.top

) t WHERE rn = 1;
来源：http://wxb.yfazqb.com

[Q35] 内连接
来源：http://cxl.havefunace.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ypt.cdnleiting.top

[Q36] 左连接
来源：http://mei.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pgu.jlsjyb.cn

[Q37] 右连接
来源：http://wce.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uhm.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://gof.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sqx.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://gkj.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fvj.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uyf.cashguo.top

[Q40] 交叉连接（笛卡尔积）
来源：http://han.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ygx.cqqwz.cn

[Q41] 多表连接
来源：http://fbc.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rrp.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://yav.ybcxt.top

JOIN products p ON p.id = o.product_id;
来源：http://ior.jinghuilouyu.cn

[Q42] 连接条件附加过滤
来源：http://imu.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://xyk.yj20258888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xju.jinqigufen.top

[Q43] 标量子查询
来源：http://tyf.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lmo.hammf.cn

[Q44] IN 子查询
来源：http://uty.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hdg.dianchejie.cn

[Q45] EXISTS 判断存在
来源：http://biw.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ibm.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nry.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vkw.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://egj.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eij.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://agm.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xlx.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://vex.jqgfzy.top

[Q49] 更新单行
来源：http://lcs.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bfw.yongpay.top

[Q50] 批量更新
来源：http://hlo.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://czv.bbcook.cn

[Q51] 用子查询更新
来源：http://hwe.shanyushiyangtech.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rco.ydzc1.top

[Q52] 删除指定行
来源：http://dtp.zhengqikj.top

DELETE FROM users WHERE id = 10;
来源：http://crh.tarul.cn

[Q53] 按条件删除
来源：http://hpx.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ksc.nanxinkj.top

[Q54] 清空表
来源：http://qne.redwolf501.top

TRUNCATE TABLE logs;
来源：http://yoi.fktsv.cn

[Q55] 排名（并列占位）
来源：http://wdo.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ywe.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://ent.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://brt.feifeiyinyue.top

[Q57] 行号
来源：http://ryh.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gpd.shanyushiyangtech.top

[Q58] 累计求和
来源：http://wlq.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tyj.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://fuc.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rmu.hammf.cn

[Q60] 取上一行 / 下一行
来源：http://ipb.ydzc1.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yyp.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uzx.epnwcf.com

[Q61] 移动平均
来源：http://cge.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cyx.aibaodan.cn

[Q62] 分组占比
来源：http://xyp.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hmn.cashguo.top

[Q63] 开启事务
来源：http://eom.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jzl.tarul.cn

[Q64] 提交事务
来源：http://wbg.nanxinkj.top

COMMIT;
来源：http://brn.jianghu66.top

[Q65] 回滚事务
来源：http://wtf.hnqzz.top

ROLLBACK;
来源：http://uzw.52xcode.cn

[Q66] 行锁查询
来源：http://otx.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mcx.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://kal.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fqn.cashguo.top

[Q68] 保存点
来源：http://wvt.mhx1999.top

SAVEPOINT sp1;
来源：http://jqk.ivvv.top

ROLLBACK TO sp1;
来源：http://quq.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://cck.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ion.pengpengdd.cyou

[Q70] 更新统计信息
来源：http://fvi.yuanzhike.top

ANALYZE TABLE users;
来源：http://bcr.birdmap.top

[Q71] 查看建表语句
来源：http://raf.fktsv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yqf.xziqi.cn

[Q72] 查看索引
来源：http://qxq.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://yzm.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://rmq.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rmy.xylfe.cn

[Q74] 强制使用索引
来源：http://lbf.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ycv.hnqzz.top

[Q75] 日期格式化
来源：http://cfl.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xhz.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qxc.zhiwuduotai.top

[Q76] 按天统计
来源：http://ohj.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cmd.hongshengwenyu.top

[Q77] 时间加减
来源：http://spw.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oeq.yangfankeji.com

[Q78] 当前时间
来源：http://rac.ppjwa.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rse.dashuyun.cn

[Q79] 字符串拼接
来源：http://afs.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ltq.fengsongda.top

[Q80] 字符串截取
来源：http://jgt.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qii.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://ith.hesvh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zgb.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://hms.cucudq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dxf.cashguo.top

[Q83] 大小写转换
来源：http://yok.52xcode.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gei.yj202588.top

[Q84] 去除首尾空格
来源：http://wnl.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://uka.gotoacloud.top

[Q85] 数值取整
来源：http://blm.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hsx.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://qod.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tap.shzxlz.cn

[Q87] JSON 字段做条件
来源：http://ytd.yangfankeji.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zdt.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://sxv.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qkw.zhongyouzk.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vfk.bjfxy.top

[Q89] 判断表是否存在
来源：http://zex.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uph.chenzaomai.com

[Q90] 生成序号列
来源：http://vkl.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tpu.yuxming.cn

================================================================================
来源：http://ovi.jyoumei.cn

R. Bash 专题
来源：http://zpv.c1oappe.top

================================================================================
来源：http://ndn.hcnkem.com

[R01] shebang 与严格模式
来源：http://eob.yj20258888.top

#!/usr/bin/env bash
来源：http://asb.hongshengwenyu.top

set -euo pipefail
来源：http://eyn.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://ytj.xylfe.cn

name="Tom"; echo "$name"
来源：http://xba.fehbvm.com

[R03] 只读变量
来源：http://utm.andypj.xyz

readonly PI=3.14
来源：http://wpi.gotoacloud.top

[R04] 位置参数
来源：http://zlh.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lxw.cdnleiting.top

[R05] 参数默认值
来源：http://fht.gzhubu.top

name="${1:-default}"
来源：http://xjx.shanyushiyangkeji.top

[R06] 判断命令是否存在
来源：http://lsq.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xuu.hesvh.cn

[R07] if 判断文件
来源：http://lxu.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zel.haohaochexian.top

[R08] 数值比较
来源：http://fcp.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://vwi.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://gfa.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cdd.fehbvm.com

[R10] 正则匹配
来源：http://dxc.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nga.dianchejie.cn

[R11] case 多分支
来源：http://tjc.tarul.cn

case "$1" in
来源：http://ebe.jinqigufen.top

start) echo "启动" ;;
来源：http://fih.yuanzhike.top

stop)  echo "停止" ;;
来源：http://ved.vehdjk.com

*)     echo "未知命令" ;;
来源：http://kgp.andypj.xyz

esac
来源：http://klu.xuetiantiany.cn

[R12] for 遍历文件
来源：http://knh.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://bja.vehdjk.com

[R13] for 计数循环
来源：http://zbc.jinqigfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://ter.vehdjk.com

[R14] C 风格 for
来源：http://thv.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zkb.shzxlz.cn

[R15] while 逐行读文件
来源：http://lpe.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://plh.hnqzz.top

[R16] until 等待条件
来源：http://wzd.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gtx.xziqi.cn

[R17] 数组定义与取值
来源：http://ywe.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://dxc.uphjek.com

[R18] 遍历数组
来源：http://uem.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hds.feifeiyinyue.top

[R19] 数组长度
来源：http://uqi.cheryme.top

echo "${#arr[@]}"
来源：http://naq.aizwys.cn

[R20] 关联数组（字典）
来源：http://fpr.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://azh.bjfxy.top

[R21] 字符串长度
来源：http://jbl.zhaomingkeji.xyz

echo "${#s}"
来源：http://tnf.ydzc1.top

[R22] 截取子串
来源：http://aov.jqgfzy.top

echo "${s:0:5}"
来源：http://jmy.havefunace.top

[R23] 字符串替换
来源：http://xqt.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://znp.ivvv.top

[R24] 大小写转换
来源：http://lxe.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cmz.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://oeq.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hbo.shanyushiyangtech.top

[R26] 命令替换
来源：http://ypc.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://aty.0kj1m.cn

[R27] 算术展开
来源：http://hpl.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://uug.hesvh.cn

[R28] 浮点运算
来源：http://lis.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://puk.tian-w.cn

[R29] 定义函数
来源：http://plu.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://krz.ybcxt.top

[R30] 函数返回状态码
来源：http://rlv.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://wod.jqgufenzy.top

[R31] 局部变量
来源：http://hdm.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://ccq.ehwqpu.com

[R32] 参数个数校验
来源：http://cbo.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://stc.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://nfy.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qqc.hywenlv.cn

[R34] 退出时清理
来源：http://zqe.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://fyp.tianlin.xyz

[R35] 后台执行并等待
来源：http://zbw.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://llu.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://qjf.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wcp.xinyue.icu

[R37] 把输出赋给变量
来源：http://osz.haohaochexian.top

files=$(ls -1)
来源：http://sef.yj202588.top

[R38] 管道串联
来源：http://zph.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://btj.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://kag.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://xue.c1oappe.top

[R40] 追加写日志
来源：http://zkw.meibo888.top

echo "log" >> out.log
来源：http://mee.chenjidiqi.icu

[R41] 丢弃输出
来源：http://rrw.meibo888.top

cmd >/dev/null 2>&1
来源：http://msu.xinyue.icu

[R42] 输入重定向
来源：http://wzi.ehwqpu.com

wc -l < a.txt
来源：http://vnm.zhiwuduotai.top

[R43] 按名字查找文件
来源：http://rts.birdmap.top

find . -name "*.log" -type f
来源：http://xoo.hywenlv.cn

[R44] 按修改时间查找
来源：http://ltb.xuanzx.com

find . -mtime -7 -type f
来源：http://xzl.zycfv.cn

[R45] 批量删除
来源：http://nuy.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://wcj.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://mfj.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fbj.gogol.net.cn

[R47] sed 单行替换
来源：http://glx.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://nyr.yuanzhike.top

[R48] awk 取指定列
来源：http://utu.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://oxm.yongpay.top

[R49] awk 带条件
来源：http://pca.yj20258.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dmq.jinghuilouyu.cn

[R50] awk 求和
来源：http://inp.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://gal.meibo888.top

[R51] 排序去重取前几
来源：http://gzl.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://mkv.yonumen.top

[R52] 统计行数
来源：http://nbb.xuanzx.com

wc -l a.txt
来源：http://rnr.hywenlv.cn

[R53] 查看文件头与实时尾
来源：http://dev.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pry.hfpthk.cn

[R54] 比较两个文件
来源：http://ftd.cqqwz.cn

diff a.txt b.txt
来源：http://eoi.dashuyun.cn

[R55] 压缩与解压
来源：http://gpv.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://beh.sjlbkw.cn

[R56] 远程拷贝
来源：http://hbb.tian-w.cn

scp file user@host:/path/
来源：http://jdk.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://bcb.zdqjudy.top

ssh user@host 'uptime'
来源：http://ywq.shuidangran.top

[R58] 下载文件
来源：http://hnn.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iqb.gogol.net.cn

[R59] 发 POST JSON
来源：http://zul.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cwu.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://wla.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://esd.daxiang520.top

[R61] 磁盘占用
来源：http://tnn.yj20258888.top

df -h;  du -sh *
来源：http://npr.jiagoushi.top

[R62] 找最占空间的文件
来源：http://hxv.meibo888.top

du -ah . | sort -rh | head -10
来源：http://mza.redwolf501.top

[R63] 内存与进程
来源：http://wkr.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://lxu.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://pkz.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://gjp.yuxming.cn

[R65] 查看端口占用
来源：http://zdp.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mna.zhiwuduotai.top

[R66] 定时任务
来源：http://aqd.nanxinkj.top

crontab -e;  crontab -l
来源：http://gjt.gzhubu.top

[R67] 生成随机十六进制串
来源：http://pcx.316326.xyz


<!-- 参考信息 -->