代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://mst.9152youxi.cn

[Q22] 排序
来源：http://two.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://flg.hammf.cn

[Q23] 分页
来源：http://bkw.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pjn.xinyue.icu

[Q24] 去重
来源：http://txk.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://pxj.c1oappe.top

[Q25] 只取前 N 条
来源：http://myi.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qvz.xylfe.cn

[Q26] 计数
来源：http://hcm.fanxiaobao.xyz

SELECT COUNT(*) FROM users;
来源：http://ngi.hywenlv.cn

[Q27] 条件计数
来源：http://yot.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://udp.yj20258.top

[Q28] 求和与平均
来源：http://czc.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uki.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://qmf.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://emk.andypj.xyz

[Q30] 分组统计
来源：http://xzy.aibaodan.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oif.sweek.top

[Q31] 分组后过滤
来源：http://rvk.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://brq.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://ojx.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cdt.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wah.chenjidiqi.icu

[Q33] 多列分组
来源：http://jsm.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mzc.sweek.top

[Q34] 每组取第一条
来源：http://bhz.shangyingyoupin.top

SELECT * FROM (
来源：http://cgs.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://juh.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://tzp.tanke756.top

[Q35] 内连接
来源：http://nou.hammf.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nkp.cucudq.cn

[Q36] 左连接
来源：http://mvb.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zhp.meibo888.top

[Q37] 右连接
来源：http://skb.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mby.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zyj.jinghuilouyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://shi.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://ndj.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://afa.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xom.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zlt.zhengqikj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sar.chenlongwang.top

[Q41] 多表连接
来源：http://lzb.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lgj.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://kqr.andypj.xyz

JOIN products p ON p.id = o.product_id;
来源：http://wcs.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://xph.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://hay.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sdi.fehbvm.com

[Q43] 标量子查询
来源：http://xur.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ewg.jinqigfzy.top

[Q44] IN 子查询
来源：http://lvt.yuanzhike.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://csa.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://klg.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://otx.yueranfly.top

[Q46] NOT EXISTS 判断不存在
来源：http://ryo.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://guo.zhixingplan.top

[Q47] 与平均值比较
来源：http://dme.jianghu66.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://peb.gzhubu.top

[Q48] CTE 公用表表达式
来源：http://opd.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://arb.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://acq.shzxlz.cn

[Q49] 更新单行
来源：http://ouw.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xbg.fanxiaobao.xyz

[Q50] 批量更新
来源：http://azn.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uwp.jqgufenzy.top

[Q51] 用子查询更新
来源：http://iaz.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wqi.hnqzz.top

[Q52] 删除指定行
来源：http://sgz.epnwcf.com

DELETE FROM users WHERE id = 10;
来源：http://who.redwolf501.top

[Q53] 按条件删除
来源：http://pwu.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://shd.xinyue.icu

[Q54] 清空表
来源：http://irq.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://glc.316326.xyz

[Q55] 排名（并列占位）
来源：http://ghw.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pby.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://lcj.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dwb.zhaomingkeji.xyz

[Q57] 行号
来源：http://mml.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wuy.yuanzhike.top

[Q58] 累计求和
来源：http://nle.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bfe.xziqi.cn

[Q59] 分组内累计
来源：http://ped.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hhn.iojbl.cn

[Q60] 取上一行 / 下一行
来源：http://pqp.ppjwa.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bph.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tgx.cucudq.cn

[Q61] 移动平均
来源：http://hhx.316326.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ehb.9152youxi.cn

[Q62] 分组占比
来源：http://vnm.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dda.yj20258888.top

[Q63] 开启事务
来源：http://ost.guannengcc.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mug.hnxiangtu.top

[Q64] 提交事务
来源：http://dvr.cucudq.cn

COMMIT;
来源：http://vpd.dianchejie.cn

[Q65] 回滚事务
来源：http://rud.mhx1999.top

ROLLBACK;
来源：http://gyr.epnwcf.com

[Q66] 行锁查询
来源：http://ohk.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sjb.zdqjudy.top

[Q67] 设置隔离级别
来源：http://pgb.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://umc.yfazqb.com

[Q68] 保存点
来源：http://rnb.316326.xyz

SAVEPOINT sp1;
来源：http://llq.shuidangran.top

ROLLBACK TO sp1;
来源：http://cqq.chenlongwang.top

[Q69] 查看执行计划
来源：http://swt.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aoq.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://nlw.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://les.cashguo.top

[Q71] 查看建表语句
来源：http://nwp.hnxiangtu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://srq.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://uza.hywenlv.cn

SHOW INDEX FROM users;
来源：http://vck.yvedp.cn

[Q73] 查看表状态
来源：http://dlu.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://lfl.dianchejie.cn

[Q74] 强制使用索引
来源：http://yev.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vqx.vehdjk.com

[Q75] 日期格式化
来源：http://nhy.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://efe.jianghu66.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aly.tian-w.cn

[Q76] 按天统计
来源：http://xba.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rat.shangyingyoupin.top

[Q77] 时间加减
来源：http://gqc.yvedp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dpj.zhoulong.xyz

[Q78] 当前时间
来源：http://pzt.xingfuxueyuan.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oga.yanxiufei.cn

[Q79] 字符串拼接
来源：http://fnf.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://efl.zhoulong.xyz

[Q80] 字符串截取
来源：http://hpr.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hgl.guannengcc.top

[Q81] 字符串替换
来源：http://jex.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rsl.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://brb.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://odu.shuidangran.top

[Q83] 大小写转换
来源：http://gja.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yjm.hnqzz.top

[Q84] 去除首尾空格
来源：http://zhl.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://kmc.jinghuilouyu.cn

[Q85] 数值取整
来源：http://gwh.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://csw.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://eam.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dsn.yueranfly.top

[Q87] JSON 字段做条件
来源：http://xyw.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://atg.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://ogq.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uar.nanxuanxn.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://noy.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://ges.gotoacloud.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hib.epnwcf.com

[Q90] 生成序号列
来源：http://jqg.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zyd.gaohongyu789.top

================================================================================
来源：http://ntu.jiagoushi.top

R. Bash 专题
来源：http://uzq.fengsongda.top

================================================================================
来源：http://uvu.cucudq.cn

[R01] shebang 与严格模式
来源：http://vyq.nanxuanxn.top

#!/usr/bin/env bash
来源：http://idz.jiagoushi.top

set -euo pipefail
来源：http://vqe.hywenlv.cn

[R02] 变量赋值与使用
来源：http://rqz.jinqigufen.top

name="Tom"; echo "$name"
来源：http://nub.jinyuanbaomall.cn

[R03] 只读变量
来源：http://euo.hesvh.cn

readonly PI=3.14
来源：http://iue.zhaomingkeji.xyz

[R04] 位置参数
来源：http://zge.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://khb.jlsjyb.cn

[R05] 参数默认值
来源：http://kxv.gzhubu.top

name="${1:-default}"
来源：http://zpq.shzxlz.cn

[R06] 判断命令是否存在
来源：http://hqv.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pih.havefunace.top

[R07] if 判断文件
来源：http://pdb.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fgw.yongpay.top

[R08] 数值比较
来源：http://hcw.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vyn.hnqzz.top

[R09] 字符串比较
来源：http://tew.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://trr.chenzaomai.com

[R10] 正则匹配
来源：http://giw.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mdb.jqgfzy.top

[R11] case 多分支
来源：http://sjn.jinghuilouyu.cn

case "$1" in
来源：http://kiw.smart0.xyz

start) echo "启动" ;;
来源：http://dys.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://roe.havefunace.top

*)     echo "未知命令" ;;
来源：http://wqo.sxryk.cn

esac
来源：http://plu.yongpay.top

[R12] for 遍历文件
来源：http://rup.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://pwc.shangyingyoupin.top

[R13] for 计数循环
来源：http://mjg.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://see.tian-w.cn

[R14] C 风格 for
来源：http://xfp.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://epd.kuanghao11.cn

[R15] while 逐行读文件
来源：http://ufs.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uml.sweek.top

[R16] until 等待条件
来源：http://zdz.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://txj.sufxvd.cn

[R17] 数组定义与取值
来源：http://rfe.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://djs.gaohongyu789.top

[R18] 遍历数组
来源：http://hgf.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://laf.jianghu66.top

[R19] 数组长度
来源：http://xds.hywenlv.cn

echo "${#arr[@]}"
来源：http://wlq.daxiang520.top

[R20] 关联数组（字典）
来源：http://nwj.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xho.sxryk.cn

[R21] 字符串长度
来源：http://uzz.yfazqb.com

echo "${#s}"
来源：http://jge.tanke756.top

[R22] 截取子串
来源：http://zsp.zdbjq.cn

echo "${s:0:5}"
来源：http://hbj.xuanzx.com

[R23] 字符串替换
来源：http://hlz.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qth.zhixingplan.top

[R24] 大小写转换
来源：http://xfi.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://kjd.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://mae.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wfo.jinqigfzy.top

[R26] 命令替换
来源：http://wbd.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://hgu.yuanzhike.top

[R27] 算术展开
来源：http://haz.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://meg.havefunace.top

[R28] 浮点运算
来源：http://xhj.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://aek.hysaishi.cn

[R29] 定义函数
来源：http://hbu.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vcz.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://ter.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://wyo.hesvh.cn

[R31] 局部变量
来源：http://zch.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://vur.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://rsh.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gwl.mhx1999.top

[R33] 捕获错误并提示行号
来源：http://wdt.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zdb.316326.xyz

[R34] 退出时清理
来源：http://okr.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://gzw.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://bww.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://egh.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://hjj.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zyn.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://lag.shzxlz.cn

files=$(ls -1)
来源：http://fxp.daxiang520.top

[R38] 管道串联
来源：http://qmj.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://uyu.sweek.top

[R39] 重定向标准输出与错误
来源：http://ksr.iojbl.cn

cmd > out.log 2>&1
来源：http://tmr.chenlongwang.top

[R40] 追加写日志
来源：http://ioy.zdqjudy.top

echo "log" >> out.log
来源：http://oht.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://cic.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://tgb.fanxiaobao.xyz

[R42] 输入重定向
来源：http://uqx.xuanzx.com

wc -l < a.txt
来源：http://elm.shzxlz.cn

[R43] 按名字查找文件
来源：http://ryo.yj20258.top

find . -name "*.log" -type f
来源：http://zyb.mhx1999.top

[R44] 按修改时间查找
来源：http://tdr.sjlbkw.cn

find . -mtime -7 -type f
来源：http://qop.tanke756.top

[R45] 批量删除
来源：http://gur.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://arp.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://kfl.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://waf.vehdjk.com

[R47] sed 单行替换
来源：http://auk.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jic.cdnleiting.top

[R48] awk 取指定列
来源：http://woe.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://pby.nanxuanxn.top

[R49] awk 带条件
来源：http://xjs.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nbp.316326.xyz

[R50] awk 求和
来源：http://nfw.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gzx.fengsongda.top

[R51] 排序去重取前几
来源：http://zpy.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lwl.yanxiufei.cn

[R52] 统计行数
来源：http://tkz.fanxiaobao.xyz

wc -l a.txt
来源：http://ipq.pycfn.com

[R53] 查看文件头与实时尾
来源：http://msf.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tvn.sjlbkw.cn

[R54] 比较两个文件
来源：http://kzu.birdmap.top

diff a.txt b.txt
来源：http://pgn.gaohongyu789.top

[R55] 压缩与解压
来源：http://fpa.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rno.cqqwz.cn

[R56] 远程拷贝
来源：http://mxl.jqgufenzy.top

scp file user@host:/path/
来源：http://vvy.tianlin.xyz

[R57] 远程执行命令
来源：http://zww.hysaishi.cn

ssh user@host 'uptime'
来源：http://shy.hcnkem.com

[R58] 下载文件
来源：http://fxu.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fxu.ehwqpu.com

[R59] 发 POST JSON
来源：http://slj.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nsv.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://nvu.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://icf.tianlin.xyz

[R61] 磁盘占用
来源：http://whu.yangfankeji.com

df -h;  du -sh *
来源：http://rry.ybcxt.top

[R62] 找最占空间的文件
来源：http://tcj.yj202588.top

du -ah . | sort -rh | head -10
来源：http://nae.gogol.net.cn

[R63] 内存与进程
来源：http://cnc.zhiwuduotai.top

free -h;  ps aux | grep nginx
来源：http://ace.jinghuilouyu.cn

[R64] 结束进程
来源：http://xlw.ywan-chungtsiang.top

kill -9 $(pgrep -f app.py)
来源：http://oso.hongshengwenyu.top

[R65] 查看端口占用
来源：http://rim.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://udt.gotoacloud.top

[R66] 定时任务
来源：http://zek.fehbvm.com

crontab -e;  crontab -l
来源：http://lzt.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://oeg.xinyue.icu

openssl rand -hex 16
来源：http://dlm.cheryme.top

[R68] 计算文件校验值
来源：http://qje.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sgt.gaohongyu789.top

[R69] 生成随机密码
来源：http://mkt.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://dwd.ydzc1.top

[R70] 时间戳与互转
来源：http://tfs.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://vkr.yvedp.cn

[R71] 日期格式化
来源：http://ezp.pengpengdd.cyou


<!-- 参考信息 -->