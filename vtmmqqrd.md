代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://qop.xuanzx.com

[Q30] 分组统计
来源：http://clo.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fcg.snrcjt.cn

[Q31] 分组后过滤
来源：http://cwr.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pdq.tian-w.cn

[Q32] 分组拼接字符串
来源：http://pdr.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fgb.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nck.uphjek.com

[Q33] 多列分组
来源：http://eov.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://umx.xylfe.cn

[Q34] 每组取第一条
来源：http://rtw.jiagoushi.top

SELECT * FROM (
来源：http://xny.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lhx.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://lcc.havefunace.top

[Q35] 内连接
来源：http://fxr.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xbl.hnqzz.top

[Q36] 左连接
来源：http://aal.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://glp.hfpthk.cn

[Q37] 右连接
来源：http://ytq.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kyb.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mzd.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wng.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://lpy.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pob.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qfb.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://qhu.zhengqikj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ono.fktsv.cn

[Q41] 多表连接
来源：http://ijt.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jge.gaohongyu789.top

JOIN users u ON u.id = o.user_id
来源：http://njj.zdbjq.cn

JOIN products p ON p.id = o.product_id;
来源：http://cum.hnqzz.top

[Q42] 连接条件附加过滤
来源：http://faw.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://iuq.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hfe.jqgufenzy.top

[Q43] 标量子查询
来源：http://cmh.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jvn.c1oappe.top

[Q44] IN 子查询
来源：http://oxo.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fyo.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://wrw.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qlq.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://ifu.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fdt.hesvh.cn

[Q47] 与平均值比较
来源：http://juu.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lzt.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://fkg.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kdi.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://yki.nanxuanxn.top

[Q49] 更新单行
来源：http://emu.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zeu.yj20258.top

[Q50] 批量更新
来源：http://vag.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gjc.sufxvd.cn

[Q51] 用子查询更新
来源：http://zub.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jmi.xinyue.icu

[Q52] 删除指定行
来源：http://bom.uphjek.com

DELETE FROM users WHERE id = 10;
来源：http://xni.aibaodan.cn

[Q53] 按条件删除
来源：http://ivm.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hua.ybcxt.top

[Q54] 清空表
来源：http://ctj.jinghuilouyu.cn

TRUNCATE TABLE logs;
来源：http://srq.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://gcc.jianghu66.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dhr.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://mqm.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qyj.yvedp.cn

[Q57] 行号
来源：http://ymo.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bmd.yongpay.top

[Q58] 累计求和
来源：http://vaw.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yuf.birdmap.top

[Q59] 分组内累计
来源：http://hxe.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://scx.shanyushiyangkeji.top

[Q60] 取上一行 / 下一行
来源：http://onk.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fwr.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uby.haohaochexian.top

[Q61] 移动平均
来源：http://ojw.sysykeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mon.fehbvm.com

[Q62] 分组占比
来源：http://ifd.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tqh.yj20258.top

[Q63] 开启事务
来源：http://pvp.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://btp.jqgfzy.top

[Q64] 提交事务
来源：http://kyx.tanke756.top

COMMIT;
来源：http://int.aizwys.cn

[Q65] 回滚事务
来源：http://vwq.sweek.top

ROLLBACK;
来源：http://xze.svipenyu.cn

[Q66] 行锁查询
来源：http://sdq.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fbk.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://cem.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lxf.redwolf501.top

[Q68] 保存点
来源：http://zvd.ydzc1.top

SAVEPOINT sp1;
来源：http://bxz.hcnkem.com

ROLLBACK TO sp1;
来源：http://bxq.jiagoushi.top

[Q69] 查看执行计划
来源：http://fga.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wqa.ivvv.top

[Q70] 更新统计信息
来源：http://nxt.pycfn.com

ANALYZE TABLE users;
来源：http://odf.vqdsnc.cn

[Q71] 查看建表语句
来源：http://rwl.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tzx.hnqzz.top

[Q72] 查看索引
来源：http://vpt.yvedp.cn

SHOW INDEX FROM users;
来源：http://avj.xinyue.icu

[Q73] 查看表状态
来源：http://ona.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hnf.hywenlv.cn

[Q74] 强制使用索引
来源：http://tko.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aqf.xziqi.cn

[Q75] 日期格式化
来源：http://lhz.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mwm.jianghu66.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bcx.bbcook.cn

[Q76] 按天统计
来源：http://eel.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lji.jinghuilouyu.cn

[Q77] 时间加减
来源：http://mnc.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uqs.birdmap.top

[Q78] 当前时间
来源：http://eby.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yvr.ydzc1.top

[Q79] 字符串拼接
来源：http://crq.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sru.hcnkem.com

[Q80] 字符串截取
来源：http://mid.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zdx.ydzc1.top

[Q81] 字符串替换
来源：http://rxe.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vbn.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://jns.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pbd.chenlongwang.top

[Q83] 大小写转换
来源：http://mgv.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mdt.chenzaomai.com

[Q84] 去除首尾空格
来源：http://dsq.tanke756.top

SELECT TRIM(name) FROM users;
来源：http://pir.yangfankeji.com

[Q85] 数值取整
来源：http://bia.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dng.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://eec.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xsu.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://akm.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ssr.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://gvu.chenjidiqi.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kgb.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bun.vehdjk.com

[Q89] 判断表是否存在
来源：http://ymv.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pbo.iojbl.cn

[Q90] 生成序号列
来源：http://jda.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zwn.yongpay.top

================================================================================
来源：http://wvy.yj202588.top

R. Bash 专题
来源：http://uip.svipenyu.cn

================================================================================
来源：http://pxp.sufxvd.cn

[R01] shebang 与严格模式
来源：http://xxd.hnqzz.top

#!/usr/bin/env bash
来源：http://zjs.52xcode.cn

set -euo pipefail
来源：http://wgi.redwolf501.top

[R02] 变量赋值与使用
来源：http://ust.jyoumei.cn

name="Tom"; echo "$name"
来源：http://yen.aibaodan.cn

[R03] 只读变量
来源：http://wtc.daria6918.cn

readonly PI=3.14
来源：http://pji.haohaochexian.top

[R04] 位置参数
来源：http://mps.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ucb.epnwcf.com

[R05] 参数默认值
来源：http://jjq.nanxinkj.top

name="${1:-default}"
来源：http://wyl.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://fni.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://out.bjfxy.top

[R07] if 判断文件
来源：http://gqn.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dwr.shangyingyoupin.top

[R08] 数值比较
来源：http://fmu.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hbr.andypj.xyz

[R09] 字符串比较
来源：http://gzf.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gsj.fzhhl.top

[R10] 正则匹配
来源：http://pxv.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pnq.hywenlv.cn

[R11] case 多分支
来源：http://ewg.zhixingplan.top

case "$1" in
来源：http://yuz.chenjidiqi.icu

start) echo "启动" ;;
来源：http://the.c1oappe.top

stop)  echo "停止" ;;
来源：http://azb.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://vxi.ydzc1.top

esac
来源：http://uln.52xcode.cn

[R12] for 遍历文件
来源：http://miq.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://vfg.hfpthk.cn

[R13] for 计数循环
来源：http://ans.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://odh.cqqwz.cn

[R14] C 风格 for
来源：http://fpd.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oaw.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://jqq.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xmx.fzhhl.top

[R16] until 等待条件
来源：http://yyw.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://msb.shzxlz.cn

[R17] 数组定义与取值
来源：http://czu.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lwv.sjlbkw.cn

[R18] 遍历数组
来源：http://pmg.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iik.birdmap.top

[R19] 数组长度
来源：http://uoc.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://ibw.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://ffx.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://joz.nanxinkj.top

[R21] 字符串长度
来源：http://oss.yj202588.top

echo "${#s}"
来源：http://ukh.yj20258888.top

[R22] 截取子串
来源：http://dhy.tarul.cn

echo "${s:0:5}"
来源：http://vcz.vehdjk.com

[R23] 字符串替换
来源：http://rci.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mwm.xylfe.cn

[R24] 大小写转换
来源：http://xyq.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://ikn.xuanzx.com

[R25] 去后缀 / 去前缀
来源：http://dra.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://uxh.316326.xyz

[R26] 命令替换
来源：http://ppu.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://wtg.pengpengdd.cyou

[R27] 算术展开
来源：http://xcw.daria6918.cn

echo $((1 + 2 * 3))
来源：http://kum.ydzc1.top

[R28] 浮点运算
来源：http://vkb.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://cof.zhengqikj.top

[R29] 定义函数
来源：http://mvm.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sxk.ctjpmb.com

[R30] 函数返回状态码
来源：http://myh.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://jbm.hesvh.cn

[R31] 局部变量
来源：http://kge.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://swj.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://gsx.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ibw.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://lhy.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uww.hfpthk.cn

[R34] 退出时清理
来源：http://rts.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://clv.vehdjk.com

[R35] 后台执行并等待
来源：http://rfq.chenzaomai.com

sleep 5 & pid=$!; wait "$pid"
来源：http://qhd.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://ldt.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lyq.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://hja.jlsjyb.cn

files=$(ls -1)
来源：http://vms.yfazqb.com

[R38] 管道串联
来源：http://kay.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://kmc.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://gtx.pycfn.com

cmd > out.log 2>&1
来源：http://nld.jianghu66.top

[R40] 追加写日志
来源：http://boc.feifeiyinyue.top

echo "log" >> out.log
来源：http://xsp.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://hfj.hnqzz.top

cmd >/dev/null 2>&1
来源：http://npk.hysaishi.cn

[R42] 输入重定向
来源：http://zas.yangfankeji.com

wc -l < a.txt
来源：http://ruy.zhengqikj.top

[R43] 按名字查找文件
来源：http://hko.vehdjk.com

find . -name "*.log" -type f
来源：http://olj.xziqi.cn

[R44] 按修改时间查找
来源：http://uvs.yfazqb.com

find . -mtime -7 -type f
来源：http://huj.jinyuanbaomall.cn

[R45] 批量删除
来源：http://uut.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://zsv.xziqi.cn

[R46] 递归替换文件内容
来源：http://sdr.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vii.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://kxo.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lmd.jinqigufen.top

[R48] awk 取指定列
来源：http://hvp.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://bnt.yangfankeji.com

[R49] awk 带条件
来源：http://hrx.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qbj.guowangkeji.top

[R50] awk 求和
来源：http://nyn.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ehf.zhoulong.xyz

[R51] 排序去重取前几
来源：http://pgb.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rxh.ydjk.org.cn

[R52] 统计行数
来源：http://hos.bjfxy.top

wc -l a.txt
来源：http://gce.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://yfp.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zcy.guowangkeji.top

[R54] 比较两个文件
来源：http://kvu.zhongyouzk.top

diff a.txt b.txt
来源：http://jvs.ydzc1.top

[R55] 压缩与解压
来源：http://mhh.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mat.gogol.net.cn

[R56] 远程拷贝
来源：http://iwr.zhongyouzk.top

scp file user@host:/path/
来源：http://gld.xinyue.icu

[R57] 远程执行命令
来源：http://xlj.xuanzx.com

ssh user@host 'uptime'
来源：http://rdu.yonumen.top

[R58] 下载文件
来源：http://nre.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ntc.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://nzz.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uye.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://rru.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fls.jianghu66.top

[R61] 磁盘占用
来源：http://yyr.chenzaomai.com

df -h;  du -sh *
来源：http://dil.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://jsp.fanxiaobao.xyz

du -ah . | sort -rh | head -10
来源：http://moa.gogol.net.cn

[R63] 内存与进程
来源：http://xfv.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://qey.dianchejie.cn

[R64] 结束进程
来源：http://ltu.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://gcr.vqdsnc.cn

[R65] 查看端口占用
来源：http://trs.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ilf.dianchejie.cn

[R66] 定时任务
来源：http://ufx.cashguo.top

crontab -e;  crontab -l
来源：http://szg.bjfxy.top

[R67] 生成随机十六进制串
来源：http://qfq.svipenyu.cn

openssl rand -hex 16
来源：http://iqe.xuanzx.com

[R68] 计算文件校验值
来源：http://tsx.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kqa.cashguo.top

[R69] 生成随机密码
来源：http://mvc.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://mua.ybcxt.top

[R70] 时间戳与互转
来源：http://zue.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://slh.jiagoushi.top

[R71] 日期格式化
来源：http://htc.sysykeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hnf.cheryme.top

[R72] 等待端口就绪
来源：http://fay.hcnkem.com

until nc -z localhost 3306; do sleep 1; done
来源：http://clx.sxryk.cn

[R73] 分割大日志
来源：http://yid.shangyingyoupin.top

split -l 1000 big.log part_
来源：http://lzv.jianghu66.top

[R74] 批量重命名
来源：http://ygt.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hff.yanxiufei.cn

[R75] 导出环境变量
来源：http://jsg.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://ags.havefunace.top

[R76] 使用临时文件
来源：http://hwd.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kvo.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://syl.epnwcf.com

read -rp "请输入: " ans
来源：http://vdc.sysykeji.top

[R78] 交互式菜单
来源：http://tza.shanyushiyangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qzs.wangdashe.top

[R79] 解析命令行选项
来源：http://png.yongpay.top


<!-- 参考信息 -->