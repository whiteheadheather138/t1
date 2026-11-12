代发 wailian999

[Q33] 多列分组
来源：http://eso.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tgw.havefunace.top

[Q34] 每组取第一条
来源：http://lsp.xylfe.cn

SELECT * FROM (
来源：http://eaf.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xjt.jqgufenzy.top

) t WHERE rn = 1;
来源：http://tjt.52xcode.cn

[Q35] 内连接
来源：http://phg.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mki.0kj1m.cn

[Q36] 左连接
来源：http://mso.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nei.pengpengdd.cyou

[Q37] 右连接
来源：http://ckz.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://chs.svipenyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lnf.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ius.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://ujb.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hmn.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oys.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pvu.snrcjt.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vua.jinghuilouyu.cn

[Q41] 多表连接
来源：http://tbn.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://elz.mhx1999.top

JOIN users u ON u.id = o.user_id
来源：http://iyq.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://nsg.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://pna.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://auk.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qft.epnwcf.com

[Q43] 标量子查询
来源：http://aco.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ltc.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://kpu.vehdjk.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lkk.jinqigufen.top

[Q45] EXISTS 判断存在
来源：http://dkp.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ouw.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iem.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dpd.cashguo.top

[Q47] 与平均值比较
来源：http://xiv.cheryme.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wqn.birdmap.top

[Q48] CTE 公用表表达式
来源：http://msz.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://muv.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://pkz.sysykeji.top

[Q49] 更新单行
来源：http://ezr.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kzc.gotoacloud.top

[Q50] 批量更新
来源：http://jpx.vehdjk.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vxa.snrcjt.cn

[Q51] 用子查询更新
来源：http://xhk.fengsongda.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cjn.zycfv.cn

[Q52] 删除指定行
来源：http://rtr.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://hku.feifeiyinyue.top

[Q53] 按条件删除
来源：http://cxu.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ibn.daxiang520.top

[Q54] 清空表
来源：http://qzo.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://dcp.gaohongyu789.top

[Q55] 排名（并列占位）
来源：http://xdx.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kbv.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://hnf.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qvb.sysykeji.top

[Q57] 行号
来源：http://vfx.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hzj.ctjpmb.com

[Q58] 累计求和
来源：http://lft.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nti.sweek.top

[Q59] 分组内累计
来源：http://syt.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gqp.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://odw.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nuk.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eky.gaohongyu789.top

[Q61] 移动平均
来源：http://gts.cqqwz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qjg.ivvv.top

[Q62] 分组占比
来源：http://fkp.zhengqikj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vyp.epnwcf.com

[Q63] 开启事务
来源：http://enx.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://jkz.wangshuangyany.cn

[Q64] 提交事务
来源：http://wiu.fanxiaobao.xyz

COMMIT;
来源：http://kcp.jinqigfzy.top

[Q65] 回滚事务
来源：http://fmh.uphjek.com

ROLLBACK;
来源：http://aye.chenzaomai.com

[Q66] 行锁查询
来源：http://bzx.epnwcf.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fia.0kj1m.cn

[Q67] 设置隔离级别
来源：http://how.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uyr.pengpengdd.cyou

[Q68] 保存点
来源：http://udj.cucudq.cn

SAVEPOINT sp1;
来源：http://kbg.hywenlv.cn

ROLLBACK TO sp1;
来源：http://uue.jlsjyb.cn

[Q69] 查看执行计划
来源：http://xti.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cgi.birdmap.top

[Q70] 更新统计信息
来源：http://pmf.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://vhx.zhongyouzk.top

[Q71] 查看建表语句
来源：http://ffn.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fvm.jianghu66.top

[Q72] 查看索引
来源：http://jte.tarul.cn

SHOW INDEX FROM users;
来源：http://bxt.52xcode.cn

[Q73] 查看表状态
来源：http://yzf.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xiv.jlsjyb.cn

[Q74] 强制使用索引
来源：http://pxp.xuetiantiany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fve.ehwqpu.com

[Q75] 日期格式化
来源：http://wec.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rbt.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dhw.hcnkem.com

[Q76] 按天统计
来源：http://pfg.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mkr.yongpay.top

[Q77] 时间加减
来源：http://jrs.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nre.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://tpq.vqdsnc.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bxy.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://djz.ybcxt.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vzi.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://bxb.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://muo.xziqi.cn

[Q81] 字符串替换
来源：http://smw.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ejy.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://dab.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ity.bbcook.cn

[Q83] 大小写转换
来源：http://voj.uphjek.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hut.hysaishi.cn

[Q84] 去除首尾空格
来源：http://erf.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://trv.feifeiyinyue.top

[Q85] 数值取整
来源：http://knq.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mgt.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://njs.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mde.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://ziw.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rfm.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://anq.xylfe.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cme.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://opl.pycfn.com

[Q89] 判断表是否存在
来源：http://wxl.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xjf.snrcjt.cn

[Q90] 生成序号列
来源：http://zmj.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ubu.c1oappe.top

================================================================================
来源：http://isr.iojbl.cn

R. Bash 专题
来源：http://dpp.mhx1999.top

================================================================================
来源：http://ugl.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://hfv.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://rsm.tian-w.cn

set -euo pipefail
来源：http://ens.chenlongwang.top

[R02] 变量赋值与使用
来源：http://pfv.jinqigufen.top

name="Tom"; echo "$name"
来源：http://enm.birdmap.top

[R03] 只读变量
来源：http://sht.0kj1m.cn

readonly PI=3.14
来源：http://fcf.zdqjudy.top

[R04] 位置参数
来源：http://ftb.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jbr.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://qqb.hesvh.cn

name="${1:-default}"
来源：http://ldw.bjfxy.top

[R06] 判断命令是否存在
来源：http://ftr.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ipe.jinqigufen.top

[R07] if 判断文件
来源：http://qzy.zhijiandao.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wui.gogol.net.cn

[R08] 数值比较
来源：http://bie.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://unr.ydzc1.top

[R09] 字符串比较
来源：http://wns.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jkk.mhx1999.top

[R10] 正则匹配
来源：http://uju.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lhh.ydzc1.top

[R11] case 多分支
来源：http://oay.xinyue.icu

case "$1" in
来源：http://mqd.daxiang520.top

start) echo "启动" ;;
来源：http://cir.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://ntb.vehdjk.com

*)     echo "未知命令" ;;
来源：http://cbv.yongpay.top

esac
来源：http://eus.bjfxy.top

[R12] for 遍历文件
来源：http://ike.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://euj.gogol.net.cn

[R13] for 计数循环
来源：http://kxu.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://udr.ybcxt.top

[R14] C 风格 for
来源：http://gqz.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hgy.hammf.cn

[R15] while 逐行读文件
来源：http://vft.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mlb.ehwqpu.com

[R16] until 等待条件
来源：http://xjo.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fnv.ivvv.top

[R17] 数组定义与取值
来源：http://nxt.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://dto.yueranfly.top

[R18] 遍历数组
来源：http://ciw.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ghf.tianlin.xyz

[R19] 数组长度
来源：http://nzo.yongpay.top

echo "${#arr[@]}"
来源：http://tya.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://fav.shanyushiyangtech.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uhg.quarkkingdee.top

[R21] 字符串长度
来源：http://mqd.hysaishi.cn

echo "${#s}"
来源：http://gvy.chenjidiqi.icu

[R22] 截取子串
来源：http://tgs.jianghu66.top

echo "${s:0:5}"
来源：http://dft.yanxiufei.cn

[R23] 字符串替换
来源：http://uqi.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aow.yj20258888.top

[R24] 大小写转换
来源：http://urt.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://xgl.andypj.xyz

[R25] 去后缀 / 去前缀
来源：http://kfo.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tcd.hnxiangtu.top

[R26] 命令替换
来源：http://swe.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://zwm.hesvh.cn

[R27] 算术展开
来源：http://hxq.tian-w.cn

echo $((1 + 2 * 3))
来源：http://zxf.52xcode.cn

[R28] 浮点运算
来源：http://pwa.zhengqikj.top

echo "scale=2; 10/3" | bc
来源：http://tri.hfpthk.cn

[R29] 定义函数
来源：http://dqb.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ofw.sweek.top

[R30] 函数返回状态码
来源：http://dkw.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://nst.shanyushiyangkeji.top

[R31] 局部变量
来源：http://jdc.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://jtl.daria6918.cn

[R32] 参数个数校验
来源：http://iue.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yqz.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://naf.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jgg.yj20258.top

[R34] 退出时清理
来源：http://kej.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ulk.zhixingplan.top

[R35] 后台执行并等待
来源：http://jso.birdmap.top

sleep 5 & pid=$!; wait "$pid"
来源：http://shx.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://zlc.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hwo.aizwys.cn

[R37] 把输出赋给变量
来源：http://prg.kuanghao11.cn

files=$(ls -1)
来源：http://aeh.shuidangran.top

[R38] 管道串联
来源：http://fid.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://vcl.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://xhe.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://zrf.gotoacloud.top

[R40] 追加写日志
来源：http://kjk.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://cmi.hnxiangtu.top

[R41] 丢弃输出
来源：http://cjl.andypj.xyz

cmd >/dev/null 2>&1
来源：http://kla.shangyingyoupin.top

[R42] 输入重定向
来源：http://sic.yvedp.cn

wc -l < a.txt
来源：http://ugf.zhixingplan.top

[R43] 按名字查找文件
来源：http://zfh.chenlongwang.top

find . -name "*.log" -type f
来源：http://utj.zdbjq.cn

[R44] 按修改时间查找
来源：http://nug.vehdjk.com

find . -mtime -7 -type f
来源：http://uxa.fzhhl.top

[R45] 批量删除
来源：http://dui.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://tdv.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://znu.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bdi.nwbrower.top

[R47] sed 单行替换
来源：http://awc.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://dee.bbcook.cn

[R48] awk 取指定列
来源：http://fog.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://rhy.jyoumei.cn

[R49] awk 带条件
来源：http://fva.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cfa.zhengqikj.top

[R50] awk 求和
来源：http://usa.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://iip.cucudq.cn

[R51] 排序去重取前几
来源：http://ixv.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://fdl.wangshuangyany.cn

[R52] 统计行数
来源：http://rrq.shanyushiyangkeji.top

wc -l a.txt
来源：http://hhk.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://tna.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://osm.ppjwa.cn

[R54] 比较两个文件
来源：http://mzl.iojbl.cn

diff a.txt b.txt
来源：http://szz.fzhhl.top

[R55] 压缩与解压
来源：http://fna.hammf.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fah.fehbvm.com

[R56] 远程拷贝
来源：http://qec.jinqigufen.top

scp file user@host:/path/
来源：http://slu.guowangkeji.top

[R57] 远程执行命令
来源：http://vhx.iojbl.cn

ssh user@host 'uptime'
来源：http://fom.guowangkeji.top

[R58] 下载文件
来源：http://kxw.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lxw.tianlin.xyz

[R59] 发 POST JSON
来源：http://zwq.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nvy.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://nnu.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zhw.zhixingplan.top

[R61] 磁盘占用
来源：http://fch.sysykeji.top

df -h;  du -sh *
来源：http://wfj.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://yid.yj202588.top

du -ah . | sort -rh | head -10
来源：http://wuw.snrcjt.cn

[R63] 内存与进程
来源：http://oac.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://tka.zhaomingkeji.xyz

[R64] 结束进程
来源：http://rcn.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://xlr.hysaishi.cn

[R65] 查看端口占用
来源：http://dzt.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vyc.sysykeji.top

[R66] 定时任务
来源：http://zcz.yongpay.top

crontab -e;  crontab -l
来源：http://xcd.tian-w.cn

[R67] 生成随机十六进制串
来源：http://pzg.smart0.xyz

openssl rand -hex 16
来源：http://jdi.zhengqikj.top

[R68] 计算文件校验值
来源：http://zck.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://add.bbcook.cn

[R69] 生成随机密码
来源：http://vad.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://mgd.hnqzz.top

[R70] 时间戳与互转
来源：http://wwq.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://xxa.hammf.cn

[R71] 日期格式化
来源：http://dyj.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://htl.nwbrower.top

[R72] 等待端口就绪
来源：http://fht.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hhu.jqgufenzy.top

[R73] 分割大日志
来源：http://zrp.hnqzz.top

split -l 1000 big.log part_
来源：http://rit.bbcook.cn

[R74] 批量重命名
来源：http://azm.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wui.ydjk.org.cn

[R75] 导出环境变量
来源：http://egi.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://hvl.aibaodan.cn

[R76] 使用临时文件
来源：http://jhx.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ntq.gzhubu.top

[R77] 读取用户输入
来源：http://foh.fktsv.cn

read -rp "请输入: " ans
来源：http://lnc.tanke756.top

[R78] 交互式菜单
来源：http://eib.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wbb.tian-w.cn

[R79] 解析命令行选项
来源：http://frz.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zfr.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://cdf.wangdashe.top

time ./run.sh
来源：http://fqa.sweek.top

================================================================================
来源：http://xzp.tarul.cn

S. C / C++ 专题
来源：http://vps.epnwcf.com

================================================================================
来源：http://pya.andypj.xyz

[S01] C：Hello World
来源：http://zjd.bbcook.cn

#include <stdio.h>
来源：http://yzg.yvedp.cn


<!-- 参考信息 -->