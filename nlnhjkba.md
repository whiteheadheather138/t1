代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uzd.hongshengwenyu.top

[Q24] 去重
来源：http://mbd.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://iaa.hammf.cn

[Q25] 只取前 N 条
来源：http://uaq.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bxx.ctjpmb.com

[Q26] 计数
来源：http://xvh.xingfuxueyuan.xyz

SELECT COUNT(*) FROM users;
来源：http://ffi.redwolf501.top

[Q27] 条件计数
来源：http://wsu.birdmap.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aoa.zhijiandao.cn

[Q28] 求和与平均
来源：http://odq.fzhhl.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cxf.guowangkeji.top

[Q29] 最大最小值
来源：http://abx.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ydr.jinqigufen.top

[Q30] 分组统计
来源：http://xcw.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kfa.yueranfly.top

[Q31] 分组后过滤
来源：http://vtk.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://met.sysykeji.top

[Q32] 分组拼接字符串
来源：http://iqr.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cpv.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rzv.vehdjk.com

[Q33] 多列分组
来源：http://xoy.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cnr.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://cdb.jianghu66.top

SELECT * FROM (
来源：http://qvn.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tfv.sufxvd.cn

) t WHERE rn = 1;
来源：http://rjb.shuidangran.top

[Q35] 内连接
来源：http://atb.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qhw.jinqigfzy.top

[Q36] 左连接
来源：http://atc.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ijj.yonumen.top

[Q37] 右连接
来源：http://xvd.daria6918.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bpu.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://epf.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zec.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://wyh.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fcp.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tsj.hcnkem.com

[Q40] 交叉连接（笛卡尔积）
来源：http://dya.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://loh.316326.xyz

[Q41] 多表连接
来源：http://ifz.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://tlc.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://akv.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://coz.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://iym.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://ldw.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://naa.shangyingyoupin.top

[Q43] 标量子查询
来源：http://peh.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jrn.yj20258.top

[Q44] IN 子查询
来源：http://vmd.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vqm.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://gyt.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://isz.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yin.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gov.gogol.net.cn

[Q47] 与平均值比较
来源：http://llv.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zje.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://rhs.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ljk.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://qzg.9152youxi.cn

[Q49] 更新单行
来源：http://agf.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pjx.chenzaomai.com

[Q50] 批量更新
来源：http://qwc.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fae.bbcook.cn

[Q51] 用子查询更新
来源：http://eph.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xms.ppjwa.cn

[Q52] 删除指定行
来源：http://djv.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://vzi.zhoulong.xyz

[Q53] 按条件删除
来源：http://nrz.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zde.tian-w.cn

[Q54] 清空表
来源：http://ssp.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://mtv.meibo888.top

[Q55] 排名（并列占位）
来源：http://ndm.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://stc.cashguo.top

[Q56] 密集排名（并列不占位）
来源：http://fnn.jlsjyb.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://taw.ehwqpu.com

[Q57] 行号
来源：http://gss.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fgt.chenjidiqi.icu

[Q58] 累计求和
来源：http://qdn.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wbi.tianlin.xyz

[Q59] 分组内累计
来源：http://gaj.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kbq.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://uah.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bfj.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xqj.tarul.cn

[Q61] 移动平均
来源：http://jzj.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mip.andypj.xyz

[Q62] 分组占比
来源：http://wkl.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://msz.zhijiandao.cn

[Q63] 开启事务
来源：http://uyb.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mwv.cdnleiting.top

[Q64] 提交事务
来源：http://pvw.yueranfly.top

COMMIT;
来源：http://vay.zhixingplan.top

[Q65] 回滚事务
来源：http://hjj.cqqwz.cn

ROLLBACK;
来源：http://tuw.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://tjz.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jkg.ydzc1.top

[Q67] 设置隔离级别
来源：http://ijs.zhongyouzk.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rms.jinqigufen.top

[Q68] 保存点
来源：http://dtg.nanxinkj.top

SAVEPOINT sp1;
来源：http://mtr.yuxming.cn

ROLLBACK TO sp1;
来源：http://emo.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://lah.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wii.epnwcf.com

[Q70] 更新统计信息
来源：http://cps.cucudq.cn

ANALYZE TABLE users;
来源：http://rga.jyoumei.cn

[Q71] 查看建表语句
来源：http://fow.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nxc.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://dmk.vehdjk.com

SHOW INDEX FROM users;
来源：http://wfl.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://zmt.snrcjt.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kaf.c1oappe.top

[Q74] 强制使用索引
来源：http://hlg.vqdsnc.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bww.pengpengdd.cyou

[Q75] 日期格式化
来源：http://iyp.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gkr.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ghi.cashguo.top

[Q76] 按天统计
来源：http://ghx.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zqa.hysaishi.cn

[Q77] 时间加减
来源：http://eyv.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ttg.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://xpw.mhx1999.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xzm.yfazqb.com

[Q79] 字符串拼接
来源：http://nfu.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bji.shzxlz.cn

[Q80] 字符串截取
来源：http://vol.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://esn.ehwqpu.com

[Q81] 字符串替换
来源：http://vvt.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jer.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://iru.gogol.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://glm.ydzc1.top

[Q83] 大小写转换
来源：http://ekz.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lvz.wangdashe.top

[Q84] 去除首尾空格
来源：http://wce.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://ceq.yanxiufei.cn

[Q85] 数值取整
来源：http://okb.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://grn.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://erd.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wvw.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://vwd.dianchejie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oln.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://hhi.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jdl.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tpw.nanxinkj.top

[Q89] 判断表是否存在
来源：http://dgg.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yod.hcnkem.com

[Q90] 生成序号列
来源：http://usr.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://top.shanyushiyangkeji.top

================================================================================
来源：http://xbi.sufxvd.cn

R. Bash 专题
来源：http://ttk.ppjwa.cn

================================================================================
来源：http://cmb.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://hwj.shangyingyoupin.top

#!/usr/bin/env bash
来源：http://sdo.52xcode.cn

set -euo pipefail
来源：http://sft.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://xkp.bbcook.cn

name="Tom"; echo "$name"
来源：http://pqw.hesvh.cn

[R03] 只读变量
来源：http://oho.xziqi.cn

readonly PI=3.14
来源：http://ika.svipenyu.cn

[R04] 位置参数
来源：http://iyx.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sph.bbcook.cn

[R05] 参数默认值
来源：http://jlz.ydjk.org.cn

name="${1:-default}"
来源：http://hqw.shanyushiyangtech.top

[R06] 判断命令是否存在
来源：http://rrc.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ztg.yvedp.cn

[R07] if 判断文件
来源：http://iot.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://btj.zhixingplan.top

[R08] 数值比较
来源：http://vav.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gqj.zhengqikj.top

[R09] 字符串比较
来源：http://lqa.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sje.chenjidiqi.icu

[R10] 正则匹配
来源：http://qqv.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qjg.bbcook.cn

[R11] case 多分支
来源：http://nhw.ppjwa.cn

case "$1" in
来源：http://frl.bbcook.cn

start) echo "启动" ;;
来源：http://edw.jinqigufen.top

stop)  echo "停止" ;;
来源：http://gtw.birdmap.top

*)     echo "未知命令" ;;
来源：http://xay.tanke756.top

esac
来源：http://sya.smart0.xyz

[R12] for 遍历文件
来源：http://cev.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://myy.ybcxt.top

[R13] for 计数循环
来源：http://jxg.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ice.cdnleiting.top

[R14] C 风格 for
来源：http://gor.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://waw.guowangkeji.top

[R15] while 逐行读文件
来源：http://aow.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pqb.meibo888.top

[R16] until 等待条件
来源：http://hhn.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://saf.shuidangran.top

[R17] 数组定义与取值
来源：http://qag.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://nlz.iojbl.cn

[R18] 遍历数组
来源：http://nkf.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bvh.zhoulong.xyz

[R19] 数组长度
来源：http://zjy.hcnkem.com

echo "${#arr[@]}"
来源：http://lav.snrcjt.cn

[R20] 关联数组（字典）
来源：http://amr.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hfa.cheryme.top

[R21] 字符串长度
来源：http://piu.316326.xyz

echo "${#s}"
来源：http://xik.zhiwuduotai.top

[R22] 截取子串
来源：http://sod.zhoulong.xyz

echo "${s:0:5}"
来源：http://rgm.jinghuilouyu.cn

[R23] 字符串替换
来源：http://aar.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iit.9152youxi.cn

[R24] 大小写转换
来源：http://aee.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://glj.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://xjj.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jnv.sysykeji.top

[R26] 命令替换
来源：http://rpe.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://nur.hammf.cn

[R27] 算术展开
来源：http://enj.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://dhl.zhoulong.xyz

[R28] 浮点运算
来源：http://zjy.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://aar.hfpthk.cn

[R29] 定义函数
来源：http://pmd.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kww.sufxvd.cn

[R30] 函数返回状态码
来源：http://lsa.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://pps.dianchejie.cn

[R31] 局部变量
来源：http://ggi.hesvh.cn

f() { local x=1; echo "$x"; }
来源：http://zwa.aizwys.cn

[R32] 参数个数校验
来源：http://dgu.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mlo.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://oja.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dwk.cqqwz.cn

[R34] 退出时清理
来源：http://yze.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mox.kuanghao11.cn

[R35] 后台执行并等待
来源：http://hue.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jvh.smart0.xyz

[R36] 并发执行多个任务
来源：http://ppy.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tfe.wangdashe.top

[R37] 把输出赋给变量
来源：http://ltv.gzhubu.top

files=$(ls -1)
来源：http://yol.xziqi.cn

[R38] 管道串联
来源：http://slk.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://wqc.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://sjm.aizwys.cn

cmd > out.log 2>&1
来源：http://lma.gogol.net.cn

[R40] 追加写日志
来源：http://swr.chenjidiqi.icu

echo "log" >> out.log
来源：http://awj.zhengqikj.top

[R41] 丢弃输出
来源：http://mnm.uphjek.com

cmd >/dev/null 2>&1
来源：http://ysc.yangfankeji.com

[R42] 输入重定向
来源：http://fbm.bjfxy.top

wc -l < a.txt
来源：http://tnu.hnqzz.top

[R43] 按名字查找文件
来源：http://znw.zhengqikj.top

find . -name "*.log" -type f
来源：http://qir.jyoumei.cn

[R44] 按修改时间查找
来源：http://vwe.andypj.xyz

find . -mtime -7 -type f
来源：http://rck.hcnkem.com

[R45] 批量删除
来源：http://onl.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://vlv.fehbvm.com

[R46] 递归替换文件内容
来源：http://mzf.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uau.feifeiyinyue.top

[R47] sed 单行替换
来源：http://ouc.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://yye.tarul.cn

[R48] awk 取指定列
来源：http://vdy.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://iox.fengsongda.top

[R49] awk 带条件
来源：http://ssd.hongshengwenyu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zkj.yueranfly.top

[R50] awk 求和
来源：http://gch.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ccf.chenlongwang.top

[R51] 排序去重取前几
来源：http://zny.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://awr.uphjek.com

[R52] 统计行数
来源：http://wrc.0kj1m.cn

wc -l a.txt
来源：http://akq.uphjek.com

[R53] 查看文件头与实时尾
来源：http://shk.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yvj.ppjwa.cn

[R54] 比较两个文件
来源：http://ppk.jinqigufen.top

diff a.txt b.txt
来源：http://bqm.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://pub.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kpg.guowangkeji.top

[R56] 远程拷贝
来源：http://tsq.vehdjk.com

scp file user@host:/path/
来源：http://nzz.zdbjq.cn

[R57] 远程执行命令
来源：http://gun.haohaochexian.top

ssh user@host 'uptime'
来源：http://zzg.cqqwz.cn

[R58] 下载文件
来源：http://bbv.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uns.redwolf501.top

[R59] 发 POST JSON
来源：http://azn.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nue.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://pst.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pvi.vehdjk.com

[R61] 磁盘占用
来源：http://pjo.svipenyu.cn

df -h;  du -sh *
来源：http://hkx.yonumen.top

[R62] 找最占空间的文件
来源：http://ojg.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://uhz.hesvh.cn

[R63] 内存与进程
来源：http://tmm.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://hln.epnwcf.com

[R64] 结束进程
来源：http://vhk.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://dst.cashguo.top

[R65] 查看端口占用
来源：http://waq.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdx.cqqwz.cn

[R66] 定时任务
来源：http://oxe.zhongyouzk.top

crontab -e;  crontab -l
来源：http://ixq.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://rni.9152youxi.cn

openssl rand -hex 16
来源：http://syf.nanxuanxn.top

[R68] 计算文件校验值
来源：http://cfl.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qwv.fehbvm.com

[R69] 生成随机密码
来源：http://abe.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://pgj.yj20258888.top

[R70] 时间戳与互转
来源：http://zit.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://six.wangshuangyany.cn

[R71] 日期格式化
来源：http://uqn.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tjd.meibo888.top

[R72] 等待端口就绪
来源：http://wun.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vam.pycfn.com

[R73] 分割大日志
来源：http://rkx.kuanghao11.cn


<!-- 参考信息 -->