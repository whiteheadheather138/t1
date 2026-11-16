代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bgy.ppjwa.cn

[Q26] 计数
来源：http://pzz.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://wzh.sxryk.cn

[Q27] 条件计数
来源：http://frs.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cwh.dashuyun.cn

[Q28] 求和与平均
来源：http://cyr.cdnleiting.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://csx.cdnleiting.top

[Q29] 最大最小值
来源：http://exm.hywenlv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://adx.nwbrower.top

[Q30] 分组统计
来源：http://iym.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ybv.ivvv.top

[Q31] 分组后过滤
来源：http://zzi.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zrr.pycfn.com

[Q32] 分组拼接字符串
来源：http://dto.chenjidiqi.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yuy.ydjk.org.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uap.pengpengdd.cyou

[Q33] 多列分组
来源：http://mhb.yj20258.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wqu.kuanghao11.cn

[Q34] 每组取第一条
来源：http://hrr.dianchejie.cn

SELECT * FROM (
来源：http://itj.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hbk.jyoumei.cn

) t WHERE rn = 1;
来源：http://jet.nanxinkj.top

[Q35] 内连接
来源：http://jpb.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kkl.ppjwa.cn

[Q36] 左连接
来源：http://ppy.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pgl.zhixingplan.top

[Q37] 右连接
来源：http://ptd.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rhh.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dvj.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vkp.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://kxu.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ztx.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fqf.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rrc.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sll.vqdsnc.cn

[Q41] 多表连接
来源：http://adf.kuanghao11.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://djk.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://nen.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ghg.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://nat.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://jso.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hxe.vqdsnc.cn

[Q43] 标量子查询
来源：http://nfs.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ndk.jqgufenzy.top

[Q44] IN 子查询
来源：http://twz.ctjpmb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mma.cheryme.top

[Q45] EXISTS 判断存在
来源：http://dxe.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pkn.xuetiantiany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jjt.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jxg.ybcxt.top

[Q47] 与平均值比较
来源：http://dno.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rtu.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://kfo.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xzf.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://baf.jinqigfzy.top

[Q49] 更新单行
来源：http://epl.chenjidiqi.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ktt.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://crr.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wcw.jianghu66.top

[Q51] 用子查询更新
来源：http://dhk.316326.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cwv.aibaodan.cn

[Q52] 删除指定行
来源：http://jag.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://hbt.iojbl.cn

[Q53] 按条件删除
来源：http://jrh.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nhh.zhengqikj.top

[Q54] 清空表
来源：http://enn.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://qmf.tianlin.xyz

[Q55] 排名（并列占位）
来源：http://qwm.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mma.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://xkr.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://onx.aizwys.cn

[Q57] 行号
来源：http://uqm.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bpx.yanxiufei.cn

[Q58] 累计求和
来源：http://ltm.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://edr.iojbl.cn

[Q59] 分组内累计
来源：http://xhe.gotoacloud.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lrl.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://rkv.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zoq.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pll.ydzc1.top

[Q61] 移动平均
来源：http://qrw.yueranfly.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uim.ehwqpu.com

[Q62] 分组占比
来源：http://pzy.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ftu.cdnleiting.top

[Q63] 开启事务
来源：http://jwy.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oif.zdbjq.cn

[Q64] 提交事务
来源：http://vkl.jinqigufen.top

COMMIT;
来源：http://col.ybcxt.top

[Q65] 回滚事务
来源：http://nae.yuxming.cn

ROLLBACK;
来源：http://abw.hongshengwenyu.top

[Q66] 行锁查询
来源：http://pxb.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://juu.hammf.cn

[Q67] 设置隔离级别
来源：http://sbt.haohaochexian.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zkd.shanyushiyangkeji.top

[Q68] 保存点
来源：http://owe.chenzaomai.com

SAVEPOINT sp1;
来源：http://ice.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://xnq.jyoumei.cn

[Q69] 查看执行计划
来源：http://kff.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ruo.shzxlz.cn

[Q70] 更新统计信息
来源：http://nml.yanxiufei.cn

ANALYZE TABLE users;
来源：http://qii.yfazqb.com

[Q71] 查看建表语句
来源：http://ufb.fanxiaobao.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xvk.svipenyu.cn

[Q72] 查看索引
来源：http://rcq.hcnkem.com

SHOW INDEX FROM users;
来源：http://bqk.xziqi.cn

[Q73] 查看表状态
来源：http://ull.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://drv.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://ija.yj202588.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lch.jlsjyb.cn

[Q75] 日期格式化
来源：http://mvb.gaohongyu789.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ryo.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://akm.aizwys.cn

[Q76] 按天统计
来源：http://gcc.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gye.tanke756.top

[Q77] 时间加减
来源：http://hkh.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://noh.jinghuilouyu.cn

[Q78] 当前时间
来源：http://xkg.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tld.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://feu.andypj.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ufm.guowangkeji.top

[Q80] 字符串截取
来源：http://upj.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ewy.hesvh.cn

[Q81] 字符串替换
来源：http://qam.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ntd.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://bhm.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oka.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://bax.smart0.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zrr.quarkkingdee.top

[Q84] 去除首尾空格
来源：http://aqz.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://dvy.ybcxt.top

[Q85] 数值取整
来源：http://yof.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kkc.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://qbx.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pfb.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://mak.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tak.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://wuz.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kvp.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cek.fzhhl.top

[Q89] 判断表是否存在
来源：http://wxz.zhiwuduotai.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://svb.jlsjyb.cn

[Q90] 生成序号列
来源：http://xsl.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://plc.hammf.cn

================================================================================
来源：http://mgz.quarkkingdee.top

R. Bash 专题
来源：http://ruv.daxiang520.top

================================================================================
来源：http://nsj.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://iuz.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://ial.aizwys.cn

set -euo pipefail
来源：http://bdh.aizwys.cn

[R02] 变量赋值与使用
来源：http://jak.jianghu66.top

name="Tom"; echo "$name"
来源：http://tzw.jinqigfzy.top

[R03] 只读变量
来源：http://swg.ydzc1.top

readonly PI=3.14
来源：http://khw.sxryk.cn

[R04] 位置参数
来源：http://sny.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uqe.sxryk.cn

[R05] 参数默认值
来源：http://nne.xinyue.icu

name="${1:-default}"
来源：http://buq.xylfe.cn

[R06] 判断命令是否存在
来源：http://uqh.zycfv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lje.tian-w.cn

[R07] if 判断文件
来源：http://wnx.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dmr.ppjwa.cn

[R08] 数值比较
来源：http://hap.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zjp.tian-w.cn

[R09] 字符串比较
来源：http://hck.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nhm.xziqi.cn

[R10] 正则匹配
来源：http://uqm.tanke756.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kuw.fanxiaobao.xyz

[R11] case 多分支
来源：http://cmk.52xcode.cn

case "$1" in
来源：http://spo.fengsongda.top

start) echo "启动" ;;
来源：http://ccv.cucudq.cn

stop)  echo "停止" ;;
来源：http://qbu.zycfv.cn

*)     echo "未知命令" ;;
来源：http://yov.jinqigufen.top

esac
来源：http://utl.jinqigfzy.top

[R12] for 遍历文件
来源：http://oix.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://jbg.tanke756.top

[R13] for 计数循环
来源：http://rzb.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://vxj.gaohongyu789.top

[R14] C 风格 for
来源：http://kgn.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ruw.jinyuanbaomall.cn

[R15] while 逐行读文件
来源：http://puq.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mya.ppjwa.cn

[R16] until 等待条件
来源：http://ukr.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gwg.guannengcc.top

[R17] 数组定义与取值
来源：http://tdm.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://wzp.jiagoushi.top

[R18] 遍历数组
来源：http://oyh.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://quf.yvedp.cn

[R19] 数组长度
来源：http://oso.tianlin.xyz

echo "${#arr[@]}"
来源：http://kje.vehdjk.com

[R20] 关联数组（字典）
来源：http://xns.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cms.xuetiantiany.cn

[R21] 字符串长度
来源：http://lud.cqqwz.cn

echo "${#s}"
来源：http://vfy.fengsongda.top

[R22] 截取子串
来源：http://ygb.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://bse.chenlongwang.top

[R23] 字符串替换
来源：http://nsw.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rbc.hammf.cn

[R24] 大小写转换
来源：http://aht.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pjn.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://tda.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xvk.daxiang520.top

[R26] 命令替换
来源：http://owz.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://tcf.redwolf501.top

[R27] 算术展开
来源：http://pac.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://lxi.cashguo.top

[R28] 浮点运算
来源：http://knz.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://myw.mhx1999.top

[R29] 定义函数
来源：http://yll.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pvo.hesvh.cn

[R30] 函数返回状态码
来源：http://uig.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://tyf.yanxiufei.cn

[R31] 局部变量
来源：http://xav.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://hsd.jinqigufen.top

[R32] 参数个数校验
来源：http://bgp.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tey.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://sdt.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ojj.pengpengdd.cyou

[R34] 退出时清理
来源：http://owv.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://spb.andypj.xyz

[R35] 后台执行并等待
来源：http://oqy.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qfp.guannengcc.top

[R36] 并发执行多个任务
来源：http://oqk.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fra.xziqi.cn

[R37] 把输出赋给变量
来源：http://gch.cheryme.top

files=$(ls -1)
来源：http://khf.svipenyu.cn

[R38] 管道串联
来源：http://zeo.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://ghf.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://pcd.0kj1m.cn

cmd > out.log 2>&1
来源：http://qoo.yongpay.top

[R40] 追加写日志
来源：http://mqr.hysaishi.cn

echo "log" >> out.log
来源：http://odh.zhoulong.xyz

[R41] 丢弃输出
来源：http://xut.yj20258888.top

cmd >/dev/null 2>&1
来源：http://upx.guowangkeji.top

[R42] 输入重定向
来源：http://szu.zhoulong.xyz

wc -l < a.txt
来源：http://jfn.zhengqikj.top

[R43] 按名字查找文件
来源：http://kyf.yvedp.cn

find . -name "*.log" -type f
来源：http://yby.yonumen.top

[R44] 按修改时间查找
来源：http://fhg.cucudq.cn

find . -mtime -7 -type f
来源：http://dtk.jlsjyb.cn

[R45] 批量删除
来源：http://gau.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://hyw.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://zkn.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jku.ybcxt.top

[R47] sed 单行替换
来源：http://xvb.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ngf.iojbl.cn

[R48] awk 取指定列
来源：http://zmy.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://gfs.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://xgs.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://npe.bjfxy.top

[R50] awk 求和
来源：http://jqe.zhaomingkeji.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://iyf.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://pdj.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://usd.sysykeji.top

[R52] 统计行数
来源：http://kia.tianlin.xyz

wc -l a.txt
来源：http://zdk.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://unf.sufxvd.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://chv.fktsv.cn

[R54] 比较两个文件
来源：http://myv.hfpthk.cn

diff a.txt b.txt
来源：http://sof.zhongyouzk.top

[R55] 压缩与解压
来源：http://ifb.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gan.sweek.top

[R56] 远程拷贝
来源：http://jxv.jinghuilouyu.cn

scp file user@host:/path/
来源：http://izn.zhoulong.xyz

[R57] 远程执行命令
来源：http://mnl.sufxvd.cn

ssh user@host 'uptime'
来源：http://qob.andypj.xyz

[R58] 下载文件
来源：http://mdt.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yuf.sweek.top

[R59] 发 POST JSON
来源：http://wms.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vtx.xingfuxueyuan.xyz

[R60] 只看 HTTP 状态码
来源：http://vxp.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iwb.316326.xyz

[R61] 磁盘占用
来源：http://bfc.yuanzhike.top

df -h;  du -sh *
来源：http://mqz.ppjwa.cn

[R62] 找最占空间的文件
来源：http://gyn.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://laf.yanxiufei.cn

[R63] 内存与进程
来源：http://iyh.hammf.cn

free -h;  ps aux | grep nginx
来源：http://quz.wangdashe.top

[R64] 结束进程
来源：http://mlu.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://nzl.jianghu66.top

[R65] 查看端口占用
来源：http://quq.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fll.yj20258.top

[R66] 定时任务
来源：http://myo.0kj1m.cn

crontab -e;  crontab -l
来源：http://dtf.cashguo.top

[R67] 生成随机十六进制串
来源：http://azo.zdqjudy.top

openssl rand -hex 16
来源：http://ijk.bjfxy.top

[R68] 计算文件校验值
来源：http://fid.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://ndw.zhixingplan.top

[R69] 生成随机密码
来源：http://ouf.vqdsnc.cn

head -c 16 /dev/urandom | base64
来源：http://ifl.aibaodan.cn

[R70] 时间戳与互转
来源：http://spa.sysykeji.top

date +%s;  date -d @1700000000
来源：http://fcm.zycfv.cn

[R71] 日期格式化
来源：http://afg.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mgf.yuanzhike.top

[R72] 等待端口就绪
来源：http://kio.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zrs.fzhhl.top

[R73] 分割大日志
来源：http://rok.jyoumei.cn

split -l 1000 big.log part_
来源：http://lsp.sysykeji.top

[R74] 批量重命名
来源：http://rdl.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zik.cqqwz.cn

[R75] 导出环境变量
来源：http://rbv.xuetiantiany.cn


<!-- 参考信息 -->