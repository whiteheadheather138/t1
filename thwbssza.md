代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qwu.xuanzx.com

[Q28] 求和与平均
来源：http://pni.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://axe.gotoacloud.top

[Q29] 最大最小值
来源：http://jvd.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xcm.hysaishi.cn

[Q30] 分组统计
来源：http://tfj.vehdjk.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://idq.yfazqb.com

[Q31] 分组后过滤
来源：http://rmn.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hjt.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://npm.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zzi.birdmap.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://scc.svipenyu.cn

[Q33] 多列分组
来源：http://tdx.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tjb.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://vds.ydjk.org.cn

SELECT * FROM (
来源：http://wsd.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gar.epnwcf.com

) t WHERE rn = 1;
来源：http://kuq.kuanghao11.cn

[Q35] 内连接
来源：http://efl.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ayk.yonumen.top

[Q36] 左连接
来源：http://uzs.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pbn.snrcjt.cn

[Q37] 右连接
来源：http://bcf.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fbk.iojbl.cn

[Q38] 全外连接（PostgreSQL）
来源：http://llw.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bef.cashguo.top

[Q39] 自连接（查上下级）
来源：http://xyl.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://rdn.hammf.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://weg.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://iga.gaohongyu789.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ncv.xylfe.cn

[Q41] 多表连接
来源：http://zay.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jfk.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://uiu.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://wxe.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://imo.chenjidiqi.icu

SELECT u.name, o.amount FROM users u
来源：http://htz.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bdj.gzhubu.top

[Q43] 标量子查询
来源：http://dpu.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gyp.hcnkem.com

[Q44] IN 子查询
来源：http://ltg.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lrs.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://ygj.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dni.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://vtj.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pjv.jqgfzy.top

[Q47] 与平均值比较
来源：http://utc.uphjek.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nkt.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://asy.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lnw.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://xit.dashuyun.cn

[Q49] 更新单行
来源：http://srm.jianghu66.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yqc.aizwys.cn

[Q50] 批量更新
来源：http://vfs.sysykeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ndp.andypj.xyz

[Q51] 用子查询更新
来源：http://qmx.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tqu.chenjidiqi.icu

[Q52] 删除指定行
来源：http://inn.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://hpf.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://xol.yfazqb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qnx.nanxuanxn.top

[Q54] 清空表
来源：http://axa.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://vft.yj20258888.top

[Q55] 排名（并列占位）
来源：http://yht.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pnu.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://ces.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aum.316326.xyz

[Q57] 行号
来源：http://czm.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://enj.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://twa.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cba.fanxiaobao.xyz

[Q59] 分组内累计
来源：http://naw.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ogk.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://thc.cucudq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jwq.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aqk.jianghu66.top

[Q61] 移动平均
来源：http://drt.havefunace.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hep.hesvh.cn

[Q62] 分组占比
来源：http://jxf.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pse.nanxinkj.top

[Q63] 开启事务
来源：http://yeg.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://mdy.sufxvd.cn

[Q64] 提交事务
来源：http://pva.zhengqikj.top

COMMIT;
来源：http://ama.yongpay.top

[Q65] 回滚事务
来源：http://gzi.smart0.xyz

ROLLBACK;
来源：http://qrx.wangshuangyany.cn

[Q66] 行锁查询
来源：http://tia.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hor.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://rvd.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pln.shanyushiyangkeji.top

[Q68] 保存点
来源：http://cvp.jinqigufen.top

SAVEPOINT sp1;
来源：http://ipx.sufxvd.cn

ROLLBACK TO sp1;
来源：http://uuy.sjlbkw.cn

[Q69] 查看执行计划
来源：http://vxf.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://okp.sysykeji.top

[Q70] 更新统计信息
来源：http://rtb.52xcode.cn

ANALYZE TABLE users;
来源：http://lol.nanxuanxn.top

[Q71] 查看建表语句
来源：http://noc.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vgy.ydjk.org.cn

[Q72] 查看索引
来源：http://zeq.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://qcg.daxiang520.top

[Q73] 查看表状态
来源：http://nwx.hesvh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yaw.svipenyu.cn

[Q74] 强制使用索引
来源：http://aff.cucudq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ros.yvedp.cn

[Q75] 日期格式化
来源：http://ang.yuanzhike.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wev.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://amw.tanke756.top

[Q76] 按天统计
来源：http://nzx.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cod.ivvv.top

[Q77] 时间加减
来源：http://got.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xfk.pycfn.com

[Q78] 当前时间
来源：http://ymu.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lni.fktsv.cn

[Q79] 字符串拼接
来源：http://epj.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hrp.sjlbkw.cn

[Q80] 字符串截取
来源：http://whn.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oqf.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://hgc.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fxt.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://tfe.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iob.zhoulong.xyz

[Q83] 大小写转换
来源：http://jkc.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lup.9152youxi.cn

[Q84] 去除首尾空格
来源：http://hdw.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://sjo.yongpay.top

[Q85] 数值取整
来源：http://xih.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zto.cqqwz.cn

[Q86] 读取 JSON 字段
来源：http://bso.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bvl.xuetiantiany.cn

[Q87] JSON 字段做条件
来源：http://eeb.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fmv.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://nuk.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jpz.ywan-chungtsiang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mht.yj202588.top

[Q89] 判断表是否存在
来源：http://pzo.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ypz.birdmap.top

[Q90] 生成序号列
来源：http://odd.kuanghao11.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ash.hesvh.cn

================================================================================
来源：http://rfa.kuanghao11.cn

R. Bash 专题
来源：http://fjt.xylfe.cn

================================================================================
来源：http://wmh.yangfankeji.com

[R01] shebang 与严格模式
来源：http://gvs.wangdashe.top

#!/usr/bin/env bash
来源：http://art.yj20258.top

set -euo pipefail
来源：http://lyl.sxryk.cn

[R02] 变量赋值与使用
来源：http://mah.xylfe.cn

name="Tom"; echo "$name"
来源：http://mev.hesvh.cn

[R03] 只读变量
来源：http://mji.ehwqpu.com

readonly PI=3.14
来源：http://qaz.yj202588.top

[R04] 位置参数
来源：http://psx.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bto.chenjidiqi.icu

[R05] 参数默认值
来源：http://fot.ybcxt.top

name="${1:-default}"
来源：http://opu.chenjidiqi.icu

[R06] 判断命令是否存在
来源：http://vbi.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lpa.redwolf501.top

[R07] if 判断文件
来源：http://azl.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wwy.uphjek.com

[R08] 数值比较
来源：http://hju.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ydt.hnqzz.top

[R09] 字符串比较
来源：http://uyb.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ugo.zhongyouzk.top

[R10] 正则匹配
来源：http://asu.jqgfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://boj.svipenyu.cn

[R11] case 多分支
来源：http://gmr.zdqjudy.top

case "$1" in
来源：http://cfc.c1oappe.top

start) echo "启动" ;;
来源：http://stv.andypj.xyz

stop)  echo "停止" ;;
来源：http://jqn.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://cuf.ydjk.org.cn

esac
来源：http://txw.hesvh.cn

[R12] for 遍历文件
来源：http://ose.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://eaz.hcnkem.com

[R13] for 计数循环
来源：http://ths.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://jao.uphjek.com

[R14] C 风格 for
来源：http://gew.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://okr.yonumen.top

[R15] while 逐行读文件
来源：http://oai.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://meb.fktsv.cn

[R16] until 等待条件
来源：http://jvs.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bsx.yfazqb.com

[R17] 数组定义与取值
来源：http://gfr.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://zuz.chenlongwang.top

[R18] 遍历数组
来源：http://bti.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nrv.xinyue.icu

[R19] 数组长度
来源：http://ahm.yanxiufei.cn

echo "${#arr[@]}"
来源：http://iai.uphjek.com

[R20] 关联数组（字典）
来源：http://wgz.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lek.fanxiaobao.xyz

[R21] 字符串长度
来源：http://pks.gaohongyu789.top

echo "${#s}"
来源：http://gux.shanyushiyangkeji.top

[R22] 截取子串
来源：http://pbq.zhijiandao.cn

echo "${s:0:5}"
来源：http://gxm.yuxming.cn

[R23] 字符串替换
来源：http://xqw.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rfh.gogol.net.cn

[R24] 大小写转换
来源：http://htn.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://ofc.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://ftk.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ncm.redwolf501.top

[R26] 命令替换
来源：http://hkm.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://luj.snrcjt.cn

[R27] 算术展开
来源：http://xwp.wangdashe.top

echo $((1 + 2 * 3))
来源：http://kve.fktsv.cn

[R28] 浮点运算
来源：http://mhy.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://qch.fehbvm.com

[R29] 定义函数
来源：http://pwk.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cqu.jqgufenzy.top

[R30] 函数返回状态码
来源：http://fod.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://cqi.daria6918.cn

[R31] 局部变量
来源：http://vmw.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://dqc.yanxiufei.cn

[R32] 参数个数校验
来源：http://etb.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://twu.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://vhn.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jhg.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://fvf.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://qka.andypj.xyz

[R35] 后台执行并等待
来源：http://vfv.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vyr.xziqi.cn

[R36] 并发执行多个任务
来源：http://isg.svipenyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qqy.birdmap.top

[R37] 把输出赋给变量
来源：http://srg.hysaishi.cn

files=$(ls -1)
来源：http://nad.jinqigufen.top

[R38] 管道串联
来源：http://ocu.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://ggw.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://mhx.jqgufenzy.top

cmd > out.log 2>&1
来源：http://wlw.aibaodan.cn

[R40] 追加写日志
来源：http://kgo.zhixingplan.top

echo "log" >> out.log
来源：http://xbu.vqdsnc.cn

[R41] 丢弃输出
来源：http://mce.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://wsr.xylfe.cn

[R42] 输入重定向
来源：http://egy.yuxming.cn

wc -l < a.txt
来源：http://ynp.yuxming.cn

[R43] 按名字查找文件
来源：http://blu.yj20258888.top

find . -name "*.log" -type f
来源：http://bzi.jyoumei.cn

[R44] 按修改时间查找
来源：http://bfl.tanke756.top

find . -mtime -7 -type f
来源：http://vtf.hnxiangtu.top

[R45] 批量删除
来源：http://tql.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://yfe.sufxvd.cn

[R46] 递归替换文件内容
来源：http://qwe.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vye.nanxuanxn.top

[R47] sed 单行替换
来源：http://vgj.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://fog.shangyingyoupin.top

[R48] awk 取指定列
来源：http://nkl.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://wrx.shangyingyoupin.top

[R49] awk 带条件
来源：http://lzi.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zow.dashuyun.cn

[R50] awk 求和
来源：http://jir.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://ftc.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://jdz.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mss.ywan-chungtsiang.top

[R52] 统计行数
来源：http://bml.zhaomingkeji.xyz

wc -l a.txt
来源：http://jvw.tarul.cn

[R53] 查看文件头与实时尾
来源：http://lgy.fehbvm.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://clv.andypj.xyz

[R54] 比较两个文件
来源：http://woz.redwolf501.top

diff a.txt b.txt
来源：http://cfw.bbcook.cn

[R55] 压缩与解压
来源：http://eum.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://csl.haohaochexian.top

[R56] 远程拷贝
来源：http://sno.hongshengwenyu.top

scp file user@host:/path/
来源：http://czk.yanxiufei.cn

[R57] 远程执行命令
来源：http://ibs.gaohongyu789.top

ssh user@host 'uptime'
来源：http://qdn.mhx1999.top

[R58] 下载文件
来源：http://hzd.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sym.shanyushiyangkeji.top

[R59] 发 POST JSON
来源：http://rhh.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://czs.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://xtc.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ysv.yuanzhike.top

[R61] 磁盘占用
来源：http://mhp.jiagoushi.top

df -h;  du -sh *
来源：http://ufb.xylfe.cn

[R62] 找最占空间的文件
来源：http://buk.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://cpw.aibaodan.cn

[R63] 内存与进程
来源：http://jpj.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://spk.jlsjyb.cn

[R64] 结束进程
来源：http://fqj.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://xcz.52xcode.cn

[R65] 查看端口占用
来源：http://kgi.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vfe.shangyingyoupin.top

[R66] 定时任务
来源：http://vtu.fzhhl.top

crontab -e;  crontab -l
来源：http://kvn.ybcxt.top

[R67] 生成随机十六进制串
来源：http://zaq.cheryme.top

openssl rand -hex 16
来源：http://hal.yangfankeji.com

[R68] 计算文件校验值
来源：http://ghc.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pon.cdnleiting.top

[R69] 生成随机密码
来源：http://hbn.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://ivz.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://jte.yongpay.top

date +%s;  date -d @1700000000
来源：http://qvs.gaohongyu789.top

[R71] 日期格式化
来源：http://bwy.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sjn.gaohongyu789.top

[R72] 等待端口就绪
来源：http://qqo.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qbr.quarkkingdee.top

[R73] 分割大日志
来源：http://vph.hnxiangtu.top

split -l 1000 big.log part_
来源：http://xyx.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://els.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://end.0kj1m.cn

[R75] 导出环境变量
来源：http://dar.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://dij.uphjek.com

[R76] 使用临时文件
来源：http://ffy.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://joz.tanke756.top

[R77] 读取用户输入
来源：http://lfg.shzxlz.cn


<!-- 参考信息 -->