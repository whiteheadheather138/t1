代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wsc.yuxming.cn

[Q18] 模糊匹配
来源：http://ktu.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qkr.zdbjq.cn

[Q19] 范围查询
来源：http://mvz.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oxy.zhengqikj.top

[Q20] IN 列表
来源：http://gnu.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mhi.yonumen.top

[Q21] 空值判断
来源：http://gpw.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://oir.mhx1999.top

[Q22] 排序
来源：http://pta.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xjm.yj20258.top

[Q23] 分页
来源：http://gnx.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cqb.ywan-chungtsiang.top

[Q24] 去重
来源：http://htm.yonumen.top

SELECT DISTINCT city FROM users;
来源：http://pns.zdqjudy.top

[Q25] 只取前 N 条
来源：http://bcw.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://efy.hnxiangtu.top

[Q26] 计数
来源：http://gql.hnxiangtu.top

SELECT COUNT(*) FROM users;
来源：http://nfg.yj20258.top

[Q27] 条件计数
来源：http://pmp.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nuq.shuidangran.top

[Q28] 求和与平均
来源：http://fvc.9152youxi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yij.yj20258.top

[Q29] 最大最小值
来源：http://ckt.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://zjd.wangdashe.top

[Q30] 分组统计
来源：http://uqh.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pkx.vehdjk.com

[Q31] 分组后过滤
来源：http://vts.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mkv.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://erh.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rum.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rhs.yongpay.top

[Q33] 多列分组
来源：http://yth.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nsq.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://gju.ywan-chungtsiang.top

SELECT * FROM (
来源：http://ifi.hywenlv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ewp.birdmap.top

) t WHERE rn = 1;
来源：http://rfm.yj202588.top

[Q35] 内连接
来源：http://hce.daxiang520.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dsx.guannengcc.top

[Q36] 左连接
来源：http://grp.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ppb.gogol.net.cn

[Q37] 右连接
来源：http://tjd.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://giy.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://fty.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oqh.zhaomingkeji.xyz

[Q39] 自连接（查上下级）
来源：http://vqt.sxryk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dbc.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rwi.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kge.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qik.dianchejie.cn

[Q41] 多表连接
来源：http://zhl.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ski.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://ejv.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://yhk.cashguo.top

[Q42] 连接条件附加过滤
来源：http://cxf.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://yik.hammf.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://asj.jqgufenzy.top

[Q43] 标量子查询
来源：http://dvr.gogol.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vmx.hesvh.cn

[Q44] IN 子查询
来源：http://zsx.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hid.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://lgx.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vkw.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://krz.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nau.bbcook.cn

[Q47] 与平均值比较
来源：http://zmx.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wot.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://xyb.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nwi.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://lzz.hywenlv.cn

[Q49] 更新单行
来源：http://hlr.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ajg.svipenyu.cn

[Q50] 批量更新
来源：http://qzz.vehdjk.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nhl.52xcode.cn

[Q51] 用子查询更新
来源：http://djo.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vhr.jqgufenzy.top

[Q52] 删除指定行
来源：http://ezj.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://ysg.sysykeji.top

[Q53] 按条件删除
来源：http://jco.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vfr.iojbl.cn

[Q54] 清空表
来源：http://edm.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://tln.ybcxt.top

[Q55] 排名（并列占位）
来源：http://rsa.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nbu.meibo888.top

[Q56] 密集排名（并列不占位）
来源：http://flc.ybcxt.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://peg.aizwys.cn

[Q57] 行号
来源：http://sto.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fjf.ybcxt.top

[Q58] 累计求和
来源：http://bav.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qme.shuidangran.top

[Q59] 分组内累计
来源：http://rak.zhijiandao.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nzj.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://tvq.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qty.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cxg.smart0.xyz

[Q61] 移动平均
来源：http://dai.birdmap.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fqt.zhongyouzk.top

[Q62] 分组占比
来源：http://lgi.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wsj.vqdsnc.cn

[Q63] 开启事务
来源：http://ivu.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rud.ctjpmb.com

[Q64] 提交事务
来源：http://nzp.havefunace.top

COMMIT;
来源：http://frn.zdqjudy.top

[Q65] 回滚事务
来源：http://lad.tarul.cn

ROLLBACK;
来源：http://rnb.yfazqb.com

[Q66] 行锁查询
来源：http://heh.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kpy.fengsongda.top

[Q67] 设置隔离级别
来源：http://hzs.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fjc.nanxuanxn.top

[Q68] 保存点
来源：http://obf.yonumen.top

SAVEPOINT sp1;
来源：http://jjw.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://zsa.yuxming.cn

[Q69] 查看执行计划
来源：http://wev.chenjidiqi.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oot.guannengcc.top

[Q70] 更新统计信息
来源：http://syd.zhixingplan.top

ANALYZE TABLE users;
来源：http://fnw.zhengqikj.top

[Q71] 查看建表语句
来源：http://aje.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zwx.hcnkem.com

[Q72] 查看索引
来源：http://bba.aibaodan.cn

SHOW INDEX FROM users;
来源：http://jlt.nanxinkj.top

[Q73] 查看表状态
来源：http://unr.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ukk.xuanzx.com

[Q74] 强制使用索引
来源：http://pul.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rjn.redwolf501.top

[Q75] 日期格式化
来源：http://bao.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://igx.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dms.bbcook.cn

[Q76] 按天统计
来源：http://ovn.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://snh.zdqjudy.top

[Q77] 时间加减
来源：http://zux.yvedp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ahh.316326.xyz

[Q78] 当前时间
来源：http://trq.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nvw.xinyue.icu

[Q79] 字符串拼接
来源：http://cwm.52xcode.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://afj.iojbl.cn

[Q80] 字符串截取
来源：http://uhb.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eps.hnqzz.top

[Q81] 字符串替换
来源：http://wwv.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kvd.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://tpx.yuxming.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gho.nanxuanxn.top

[Q83] 大小写转换
来源：http://fum.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sez.cashguo.top

[Q84] 去除首尾空格
来源：http://fkd.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://jwd.ybcxt.top

[Q85] 数值取整
来源：http://ahh.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kbw.pycfn.com

[Q86] 读取 JSON 字段
来源：http://cnq.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hha.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://zxs.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://riq.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://gyy.bbcook.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hsp.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cou.zhixingplan.top

[Q89] 判断表是否存在
来源：http://kzn.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ccj.cqqwz.cn

[Q90] 生成序号列
来源：http://xev.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sgr.andypj.xyz

================================================================================
来源：http://wjz.fktsv.cn

R. Bash 专题
来源：http://xbq.yueranfly.top

================================================================================
来源：http://dui.yuanzhike.top

[R01] shebang 与严格模式
来源：http://vqe.guannengcc.top

#!/usr/bin/env bash
来源：http://amz.yj20258.top

set -euo pipefail
来源：http://sje.sysykeji.top

[R02] 变量赋值与使用
来源：http://olm.quarkkingdee.top

name="Tom"; echo "$name"
来源：http://nei.0kj1m.cn

[R03] 只读变量
来源：http://fpw.fzhhl.top

readonly PI=3.14
来源：http://fgm.hesvh.cn

[R04] 位置参数
来源：http://xzl.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://why.vqdsnc.cn

[R05] 参数默认值
来源：http://yca.zhiwuduotai.top

name="${1:-default}"
来源：http://tdj.gogol.net.cn

[R06] 判断命令是否存在
来源：http://sbl.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hgu.uphjek.com

[R07] if 判断文件
来源：http://ipd.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xib.chenjidiqi.icu

[R08] 数值比较
来源：http://uyo.ybcxt.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jfj.52xcode.cn

[R09] 字符串比较
来源：http://ldn.jinqigfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://opr.havefunace.top

[R10] 正则匹配
来源：http://glp.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mzz.shuidangran.top

[R11] case 多分支
来源：http://hgx.chenjidiqi.icu

case "$1" in
来源：http://rez.chenlongwang.top

start) echo "启动" ;;
来源：http://xqr.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://qsx.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://jfj.yvedp.cn

esac
来源：http://ays.cucudq.cn

[R12] for 遍历文件
来源：http://cvx.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://gwf.sysykeji.top

[R13] for 计数循环
来源：http://blr.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://ijh.cucudq.cn

[R14] C 风格 for
来源：http://tix.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dyi.xziqi.cn

[R15] while 逐行读文件
来源：http://gis.fzhhl.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eot.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://bxu.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://stm.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://wux.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://cxa.zhiwuduotai.top

[R18] 遍历数组
来源：http://fzk.fengsongda.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ohn.iojbl.cn

[R19] 数组长度
来源：http://bnm.316326.xyz

echo "${#arr[@]}"
来源：http://llh.aizwys.cn

[R20] 关联数组（字典）
来源：http://dny.ywan-chungtsiang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gty.sufxvd.cn

[R21] 字符串长度
来源：http://psf.xingfuxueyuan.xyz

echo "${#s}"
来源：http://bjt.sufxvd.cn

[R22] 截取子串
来源：http://cnz.yanxiufei.cn

echo "${s:0:5}"
来源：http://mfq.cucudq.cn

[R23] 字符串替换
来源：http://fpv.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://btl.hysaishi.cn

[R24] 大小写转换
来源：http://bzk.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ccc.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://qpx.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ujq.tian-w.cn

[R26] 命令替换
来源：http://vys.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://pxu.tian-w.cn

[R27] 算术展开
来源：http://xwt.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://rns.svipenyu.cn

[R28] 浮点运算
来源：http://hmk.yonumen.top

echo "scale=2; 10/3" | bc
来源：http://ltv.dianchejie.cn

[R29] 定义函数
来源：http://ghm.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jbx.cheryme.top

[R30] 函数返回状态码
来源：http://gta.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://byl.xinyue.icu

[R31] 局部变量
来源：http://pag.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://yhd.zycfv.cn

[R32] 参数个数校验
来源：http://yjt.havefunace.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kxy.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://yar.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://okq.jqgfzy.top

[R34] 退出时清理
来源：http://bmn.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://ozn.dianchejie.cn

[R35] 后台执行并等待
来源：http://iri.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ntg.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://oab.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zky.xuanzx.com

[R37] 把输出赋给变量
来源：http://pok.tianlin.xyz

files=$(ls -1)
来源：http://mjd.shangyingyoupin.top

[R38] 管道串联
来源：http://zvw.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://rof.meibo888.top

[R39] 重定向标准输出与错误
来源：http://phz.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://vip.gogol.net.cn

[R40] 追加写日志
来源：http://zuv.zycfv.cn

echo "log" >> out.log
来源：http://bei.yj20258.top

[R41] 丢弃输出
来源：http://tph.aibaodan.cn

cmd >/dev/null 2>&1
来源：http://icx.wangdashe.top

[R42] 输入重定向
来源：http://txv.sweek.top

wc -l < a.txt
来源：http://fkt.zhixingplan.top

[R43] 按名字查找文件
来源：http://hmg.epnwcf.com

find . -name "*.log" -type f
来源：http://lpa.guowangkeji.top

[R44] 按修改时间查找
来源：http://rnf.zhijiandao.cn

find . -mtime -7 -type f
来源：http://xhp.aibaodan.cn

[R45] 批量删除
来源：http://vrr.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://qub.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://wxc.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lop.havefunace.top

[R47] sed 单行替换
来源：http://wlf.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://xlp.aizwys.cn

[R48] awk 取指定列
来源：http://odl.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://zyg.gaohongyu789.top

[R49] awk 带条件
来源：http://abd.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tyb.tian-w.cn

[R50] awk 求和
来源：http://jmn.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://zqe.sxryk.cn

[R51] 排序去重取前几
来源：http://nhu.hcnkem.com

sort a.txt | uniq -c | sort -rn | head
来源：http://eku.jianghu66.top

[R52] 统计行数
来源：http://iep.snrcjt.cn

wc -l a.txt
来源：http://hpz.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://ndj.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iql.xinyue.icu

[R54] 比较两个文件
来源：http://udn.yj202588.top

diff a.txt b.txt
来源：http://zgm.yanxiufei.cn

[R55] 压缩与解压
来源：http://vbi.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hdp.ydjk.org.cn

[R56] 远程拷贝
来源：http://civ.ppjwa.cn

scp file user@host:/path/
来源：http://vcn.hnxiangtu.top

[R57] 远程执行命令
来源：http://qpl.xinyue.icu

ssh user@host 'uptime'
来源：http://asm.epnwcf.com

[R58] 下载文件
来源：http://mgg.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mtz.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://kwm.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wnm.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://chr.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lcd.xuanzx.com

[R61] 磁盘占用
来源：http://fit.zhixingplan.top

df -h;  du -sh *
来源：http://fot.chenlongwang.top

[R62] 找最占空间的文件
来源：http://air.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://ker.redwolf501.top

[R63] 内存与进程
来源：http://joc.yongpay.top

free -h;  ps aux | grep nginx
来源：http://hsb.zycfv.cn

[R64] 结束进程
来源：http://rxp.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://lbx.hywenlv.cn

[R65] 查看端口占用
来源：http://uas.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lth.hammf.cn

[R66] 定时任务
来源：http://tsl.zdqjudy.top

crontab -e;  crontab -l
来源：http://enj.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://ozw.guannengcc.top


<!-- 参考信息 -->