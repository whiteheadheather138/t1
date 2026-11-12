代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://cpl.epnwcf.com

[Q30] 分组统计
来源：http://fok.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://som.yuxming.cn

[Q31] 分组后过滤
来源：http://zts.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xrt.hcnkem.com

[Q32] 分组拼接字符串
来源：http://wbd.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zoh.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nbt.guowangkeji.top

[Q33] 多列分组
来源：http://sac.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qit.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://gis.yuxming.cn

SELECT * FROM (
来源：http://ixw.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wxb.cqqwz.cn

) t WHERE rn = 1;
来源：http://kpn.zhaomingkeji.xyz

[Q35] 内连接
来源：http://ibz.quarkkingdee.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jmv.52xcode.cn

[Q36] 左连接
来源：http://drq.gzhubu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fva.iojbl.cn

[Q37] 右连接
来源：http://lkg.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dpt.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://xvl.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kyq.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://lbt.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jos.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mbh.cqqwz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vee.haohaochexian.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sef.mhx1999.top

[Q41] 多表连接
来源：http://lhh.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://anp.aizwys.cn

JOIN users u ON u.id = o.user_id
来源：http://tzm.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://opq.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://rof.kuanghao11.cn

SELECT u.name, o.amount FROM users u
来源：http://uaj.shangyingyoupin.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oxj.yj20258888.top

[Q43] 标量子查询
来源：http://elp.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pcv.epnwcf.com

[Q44] IN 子查询
来源：http://ykr.hysaishi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kkr.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://osh.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gkd.316326.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://svp.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xmz.zhoulong.xyz

[Q47] 与平均值比较
来源：http://jqd.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tjr.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://uak.hesvh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://enq.hesvh.cn

SELECT * FROM t WHERE c > 5;
来源：http://yil.chenzaomai.com

[Q49] 更新单行
来源：http://gmp.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tel.zhiwuduotai.top

[Q50] 批量更新
来源：http://ghn.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kli.vqdsnc.cn

[Q51] 用子查询更新
来源：http://byg.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://keq.mhx1999.top

[Q52] 删除指定行
来源：http://nvd.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://scd.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://iub.pengpengdd.cyou

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lec.epnwcf.com

[Q54] 清空表
来源：http://kbm.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://uza.yfazqb.com

[Q55] 排名（并列占位）
来源：http://owm.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tzm.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://xem.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pvs.kuanghao11.cn

[Q57] 行号
来源：http://zfs.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oox.vehdjk.com

[Q58] 累计求和
来源：http://aum.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cii.tanke756.top

[Q59] 分组内累计
来源：http://wwm.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aya.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://uxj.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kzf.jyoumei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dbd.yfazqb.com

[Q61] 移动平均
来源：http://qyv.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bll.nanxuanxn.top

[Q62] 分组占比
来源：http://mpn.zhengqikj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rvv.c1oappe.top

[Q63] 开启事务
来源：http://iqw.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tdf.sufxvd.cn

[Q64] 提交事务
来源：http://wxx.hongshengwenyu.top

COMMIT;
来源：http://vyh.yfazqb.com

[Q65] 回滚事务
来源：http://xrd.hnqzz.top

ROLLBACK;
来源：http://gpx.xziqi.cn

[Q66] 行锁查询
来源：http://emy.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kul.fengsongda.top

[Q67] 设置隔离级别
来源：http://gtc.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://set.yanxiufei.cn

[Q68] 保存点
来源：http://ney.yanxiufei.cn

SAVEPOINT sp1;
来源：http://cvx.shanyushiyangkeji.top

ROLLBACK TO sp1;
来源：http://ith.yuanzhike.top

[Q69] 查看执行计划
来源：http://sgw.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pyz.hnqzz.top

[Q70] 更新统计信息
来源：http://obr.xuetiantiany.cn

ANALYZE TABLE users;
来源：http://jxn.gaohongyu789.top

[Q71] 查看建表语句
来源：http://qgm.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://shc.zhiwuduotai.top

[Q72] 查看索引
来源：http://pzo.ydzc1.top

SHOW INDEX FROM users;
来源：http://xal.hnqzz.top

[Q73] 查看表状态
来源：http://jdo.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ssh.sxryk.cn

[Q74] 强制使用索引
来源：http://pxl.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://prn.gotoacloud.top

[Q75] 日期格式化
来源：http://wak.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ufn.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rkr.jinqigufen.top

[Q76] 按天统计
来源：http://zob.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gzg.hnxiangtu.top

[Q77] 时间加减
来源：http://ovk.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hhg.pycfn.com

[Q78] 当前时间
来源：http://cbj.cheryme.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yed.yj20258888.top

[Q79] 字符串拼接
来源：http://rgf.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://swc.iojbl.cn

[Q80] 字符串截取
来源：http://ggx.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yez.yj20258.top

[Q81] 字符串替换
来源：http://nfs.xziqi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vvn.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://zjb.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eke.mhx1999.top

[Q83] 大小写转换
来源：http://nfl.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mlr.jlsjyb.cn

[Q84] 去除首尾空格
来源：http://ewg.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://xao.zhongyouzk.top

[Q85] 数值取整
来源：http://odi.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jtq.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://haw.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uue.snrcjt.cn

[Q87] JSON 字段做条件
来源：http://rsi.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bft.wangdashe.top

[Q88] 行转列（条件聚合）
来源：http://cmy.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ili.ivvv.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mwr.sweek.top

[Q89] 判断表是否存在
来源：http://bqg.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qwo.sweek.top

[Q90] 生成序号列
来源：http://eyn.xuanzx.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kyf.ivvv.top

================================================================================
来源：http://irm.c1oappe.top

R. Bash 专题
来源：http://tnn.zhoulong.xyz

================================================================================
来源：http://ixt.yfazqb.com

[R01] shebang 与严格模式
来源：http://xnw.aizwys.cn

#!/usr/bin/env bash
来源：http://har.wangshuangyany.cn

set -euo pipefail
来源：http://yjc.ydzc1.top

[R02] 变量赋值与使用
来源：http://wmm.yvedp.cn

name="Tom"; echo "$name"
来源：http://vqx.c1oappe.top

[R03] 只读变量
来源：http://yro.nanxuanxn.top

readonly PI=3.14
来源：http://hgs.sjlbkw.cn

[R04] 位置参数
来源：http://bfs.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uti.sweek.top

[R05] 参数默认值
来源：http://pnz.jlsjyb.cn

name="${1:-default}"
来源：http://hir.andypj.xyz

[R06] 判断命令是否存在
来源：http://vri.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ora.nanxinkj.top

[R07] if 判断文件
来源：http://vpa.andypj.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ncf.cheryme.top

[R08] 数值比较
来源：http://aui.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hyf.tanke756.top

[R09] 字符串比较
来源：http://btf.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qiz.zhoulong.xyz

[R10] 正则匹配
来源：http://fat.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fec.fengsongda.top

[R11] case 多分支
来源：http://uee.hcnkem.com

case "$1" in
来源：http://iun.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://fbd.redwolf501.top

stop)  echo "停止" ;;
来源：http://meh.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://vjo.316326.xyz

esac
来源：http://gbp.redwolf501.top

[R12] for 遍历文件
来源：http://aal.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://yfk.epnwcf.com

[R13] for 计数循环
来源：http://tiq.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://khn.jinqigfzy.top

[R14] C 风格 for
来源：http://dyl.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hsp.zycfv.cn

[R15] while 逐行读文件
来源：http://zmo.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://grx.fktsv.cn

[R16] until 等待条件
来源：http://yqg.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://asr.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://vlh.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://pxa.fengsongda.top

[R18] 遍历数组
来源：http://ync.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jny.smart0.xyz

[R19] 数组长度
来源：http://zcw.ctjpmb.com

echo "${#arr[@]}"
来源：http://uap.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://hri.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://whb.ivvv.top

[R21] 字符串长度
来源：http://qly.nanxinkj.top

echo "${#s}"
来源：http://lmy.xuetiantiany.cn

[R22] 截取子串
来源：http://pqe.jlsjyb.cn

echo "${s:0:5}"
来源：http://jvu.yuxming.cn

[R23] 字符串替换
来源：http://tjl.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tlp.tian-w.cn

[R24] 大小写转换
来源：http://cso.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://vkx.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://xhb.chenjidiqi.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://hgq.zycfv.cn

[R26] 命令替换
来源：http://pal.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://hqn.cucudq.cn

[R27] 算术展开
来源：http://ioe.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://vvz.haohaochexian.top

[R28] 浮点运算
来源：http://mrj.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://ylb.ywan-chungtsiang.top

[R29] 定义函数
来源：http://gwt.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jmp.sjlbkw.cn

[R30] 函数返回状态码
来源：http://uvm.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://joq.ywan-chungtsiang.top

[R31] 局部变量
来源：http://ibq.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://lns.yfazqb.com

[R32] 参数个数校验
来源：http://dwk.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ach.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://agc.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hba.yj202588.top

[R34] 退出时清理
来源：http://wdv.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sdt.c1oappe.top

[R35] 后台执行并等待
来源：http://cmq.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dwl.gotoacloud.top

[R36] 并发执行多个任务
来源：http://cfe.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rfg.tianlin.xyz

[R37] 把输出赋给变量
来源：http://ner.dashuyun.cn

files=$(ls -1)
来源：http://xlr.daria6918.cn

[R38] 管道串联
来源：http://sru.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://sjw.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://lcc.aizwys.cn

cmd > out.log 2>&1
来源：http://xia.yuanzhike.top

[R40] 追加写日志
来源：http://tjz.zdqjudy.top

echo "log" >> out.log
来源：http://eip.hysaishi.cn

[R41] 丢弃输出
来源：http://cye.cashguo.top

cmd >/dev/null 2>&1
来源：http://bar.hnxiangtu.top

[R42] 输入重定向
来源：http://bjd.hcnkem.com

wc -l < a.txt
来源：http://ebw.9152youxi.cn

[R43] 按名字查找文件
来源：http://aer.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://ulb.aibaodan.cn

[R44] 按修改时间查找
来源：http://qsc.dashuyun.cn

find . -mtime -7 -type f
来源：http://mzy.hnxiangtu.top

[R45] 批量删除
来源：http://rzn.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://psz.gzhubu.top

[R46] 递归替换文件内容
来源：http://dbu.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qyd.fengsongda.top

[R47] sed 单行替换
来源：http://uts.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://zzl.zhongyouzk.top

[R48] awk 取指定列
来源：http://xxq.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://lvt.chenjidiqi.icu

[R49] awk 带条件
来源：http://uuw.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wkj.yj20258888.top

[R50] awk 求和
来源：http://qbl.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://etn.uphjek.com

[R51] 排序去重取前几
来源：http://pjg.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mhp.nwbrower.top

[R52] 统计行数
来源：http://oix.chenzaomai.com

wc -l a.txt
来源：http://sqq.cheryme.top

[R53] 查看文件头与实时尾
来源：http://wiq.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fom.yj202588.top

[R54] 比较两个文件
来源：http://pqa.yj20258.top

diff a.txt b.txt
来源：http://tzn.ivvv.top

[R55] 压缩与解压
来源：http://zkz.yfazqb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tqb.shzxlz.cn

[R56] 远程拷贝
来源：http://xxn.chenlongwang.top

scp file user@host:/path/
来源：http://krw.guowangkeji.top

[R57] 远程执行命令
来源：http://wfa.sweek.top

ssh user@host 'uptime'
来源：http://umx.shuidangran.top

[R58] 下载文件
来源：http://ocu.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mur.jqgufenzy.top

[R59] 发 POST JSON
来源：http://tei.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tkh.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://udy.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://djd.xziqi.cn

[R61] 磁盘占用
来源：http://rqf.fanxiaobao.xyz

df -h;  du -sh *
来源：http://bpg.gogol.net.cn

[R62] 找最占空间的文件
来源：http://luf.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://vti.meibo888.top

[R63] 内存与进程
来源：http://uqp.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://pwk.fengsongda.top

[R64] 结束进程
来源：http://umq.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://wsq.wangdashe.top

[R65] 查看端口占用
来源：http://hey.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lvm.yj20258888.top

[R66] 定时任务
来源：http://sed.gotoacloud.top

crontab -e;  crontab -l
来源：http://kdr.pycfn.com

[R67] 生成随机十六进制串
来源：http://crl.smart0.xyz

openssl rand -hex 16
来源：http://nin.jqgufenzy.top

[R68] 计算文件校验值
来源：http://tqx.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://umr.ppjwa.cn

[R69] 生成随机密码
来源：http://xof.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://zwm.c1oappe.top

[R70] 时间戳与互转
来源：http://jsw.uphjek.com

date +%s;  date -d @1700000000
来源：http://hcz.zhongyouzk.top

[R71] 日期格式化
来源：http://uwq.xuetiantiany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jbk.zdqjudy.top

[R72] 等待端口就绪
来源：http://buu.xziqi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nvz.yueranfly.top

[R73] 分割大日志
来源：http://nyj.dianchejie.cn

split -l 1000 big.log part_
来源：http://mmp.epnwcf.com

[R74] 批量重命名
来源：http://ubn.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wws.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://zsl.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://jzb.zhoulong.xyz

[R76] 使用临时文件
来源：http://tdc.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eri.9152youxi.cn

[R77] 读取用户输入
来源：http://zgn.cqqwz.cn

read -rp "请输入: " ans
来源：http://vyv.yfazqb.com

[R78] 交互式菜单
来源：http://cht.ywan-chungtsiang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vci.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://xxk.shangyingyoupin.top


<!-- 参考信息 -->