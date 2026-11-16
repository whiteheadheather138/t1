代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://tsp.bjfxy.top

[Q30] 分组统计
来源：http://asa.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ybu.gotoacloud.top

[Q31] 分组后过滤
来源：http://qts.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vch.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://mza.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://urn.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nid.cheryme.top

[Q33] 多列分组
来源：http://nlz.ywan-chungtsiang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gme.sweek.top

[Q34] 每组取第一条
来源：http://dof.ydjk.org.cn

SELECT * FROM (
来源：http://gpl.cqqwz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ium.yj202588.top

) t WHERE rn = 1;
来源：http://euv.c1oappe.top

[Q35] 内连接
来源：http://odq.snrcjt.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jyb.ppjwa.cn

[Q36] 左连接
来源：http://rqi.gogol.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hbx.xingfuxueyuan.xyz

[Q37] 右连接
来源：http://lzb.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://veg.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://jmf.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://acu.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://yvo.shangyingyoupin.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jaz.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oxh.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ozb.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gyt.shzxlz.cn

[Q41] 多表连接
来源：http://pja.dashuyun.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://efi.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://cgv.jianghu66.top

JOIN products p ON p.id = o.product_id;
来源：http://jkj.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://kyh.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://sre.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jhk.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://pob.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rms.ppjwa.cn

[Q44] IN 子查询
来源：http://ooc.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xmq.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://pjs.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ezk.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://myb.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bsa.dashuyun.cn

[Q47] 与平均值比较
来源：http://eck.smart0.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jgo.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://fiq.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bon.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://lta.jinghuilouyu.cn

[Q49] 更新单行
来源：http://iwv.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yep.sufxvd.cn

[Q50] 批量更新
来源：http://iid.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wdh.ivvv.top

[Q51] 用子查询更新
来源：http://zrr.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xas.zdbjq.cn

[Q52] 删除指定行
来源：http://rtt.hnqzz.top

DELETE FROM users WHERE id = 10;
来源：http://sou.birdmap.top

[Q53] 按条件删除
来源：http://lme.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yzd.52xcode.cn

[Q54] 清空表
来源：http://ohs.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://eeo.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://hse.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tqs.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://cmv.chenzaomai.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ovj.epnwcf.com

[Q57] 行号
来源：http://tvr.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vkw.redwolf501.top

[Q58] 累计求和
来源：http://cme.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dvy.hnqzz.top

[Q59] 分组内累计
来源：http://tzo.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sba.hysaishi.cn

[Q60] 取上一行 / 下一行
来源：http://fcq.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bst.pycfn.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://esb.wangdashe.top

[Q61] 移动平均
来源：http://ieb.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cbb.0kj1m.cn

[Q62] 分组占比
来源：http://bvy.jianghu66.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jzl.hywenlv.cn

[Q63] 开启事务
来源：http://oic.hysaishi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zyw.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://jsm.jinqigfzy.top

COMMIT;
来源：http://uqo.yvedp.cn

[Q65] 回滚事务
来源：http://que.hnxiangtu.top

ROLLBACK;
来源：http://jle.pycfn.com

[Q66] 行锁查询
来源：http://pce.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vpd.wangdashe.top

[Q67] 设置隔离级别
来源：http://xog.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://twp.chenzaomai.com

[Q68] 保存点
来源：http://qkk.sweek.top

SAVEPOINT sp1;
来源：http://nww.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://tjl.birdmap.top

[Q69] 查看执行计划
来源：http://nrs.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ltc.iojbl.cn

[Q70] 更新统计信息
来源：http://pcu.xylfe.cn

ANALYZE TABLE users;
来源：http://qdx.yuxming.cn

[Q71] 查看建表语句
来源：http://cbe.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jap.tarul.cn

[Q72] 查看索引
来源：http://jtv.smart0.xyz

SHOW INDEX FROM users;
来源：http://hgl.tarul.cn

[Q73] 查看表状态
来源：http://tga.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ric.316326.xyz

[Q74] 强制使用索引
来源：http://pxa.zhiwuduotai.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uqc.yj20258888.top

[Q75] 日期格式化
来源：http://dbc.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kov.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ner.bbcook.cn

[Q76] 按天统计
来源：http://kpk.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mro.ybcxt.top

[Q77] 时间加减
来源：http://hqc.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tok.tanke756.top

[Q78] 当前时间
来源：http://cwj.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fjk.guowangkeji.top

[Q79] 字符串拼接
来源：http://vjx.yfazqb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vbb.zhoulong.xyz

[Q80] 字符串截取
来源：http://ztl.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gxi.hongshengwenyu.top

[Q81] 字符串替换
来源：http://tix.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://asg.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://ojq.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wui.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://ztp.gogol.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kur.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://gxv.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://cfi.xylfe.cn

[Q85] 数值取整
来源：http://jim.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lqc.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://fgr.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qhj.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://ttd.hysaishi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hvk.52xcode.cn

[Q88] 行转列（条件聚合）
来源：http://bku.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dgd.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mcr.gzhubu.top

[Q89] 判断表是否存在
来源：http://bqd.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zxk.jinqigufen.top

[Q90] 生成序号列
来源：http://qpd.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zty.vqdsnc.cn

================================================================================
来源：http://zee.svipenyu.cn

R. Bash 专题
来源：http://qwp.cqqwz.cn

================================================================================
来源：http://dae.epnwcf.com

[R01] shebang 与严格模式
来源：http://skl.sufxvd.cn

#!/usr/bin/env bash
来源：http://vfx.ybcxt.top

set -euo pipefail
来源：http://gka.smart0.xyz

[R02] 变量赋值与使用
来源：http://ofk.yangfankeji.com

name="Tom"; echo "$name"
来源：http://ypb.svipenyu.cn

[R03] 只读变量
来源：http://tiu.cashguo.top

readonly PI=3.14
来源：http://bil.jinqigufen.top

[R04] 位置参数
来源：http://rjk.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wbt.yueranfly.top

[R05] 参数默认值
来源：http://hsb.vehdjk.com

name="${1:-default}"
来源：http://pph.yueranfly.top

[R06] 判断命令是否存在
来源：http://skq.svipenyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yie.wangshuangyany.cn

[R07] if 判断文件
来源：http://hpx.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://phc.tarul.cn

[R08] 数值比较
来源：http://qdt.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cmv.jianghu66.top

[R09] 字符串比较
来源：http://gzo.yangfankeji.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://flt.tarul.cn

[R10] 正则匹配
来源：http://vmf.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zqz.xuanzx.com

[R11] case 多分支
来源：http://imn.aizwys.cn

case "$1" in
来源：http://yha.sjlbkw.cn

start) echo "启动" ;;
来源：http://flp.cdnleiting.top

stop)  echo "停止" ;;
来源：http://ooi.daxiang520.top

*)     echo "未知命令" ;;
来源：http://ref.ydjk.org.cn

esac
来源：http://ncs.cqqwz.cn

[R12] for 遍历文件
来源：http://haz.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://xav.chenlongwang.top

[R13] for 计数循环
来源：http://aam.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://yeg.dianchejie.cn

[R14] C 风格 for
来源：http://hpn.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fvq.yj20258.top

[R15] while 逐行读文件
来源：http://nax.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oni.yanxiufei.cn

[R16] until 等待条件
来源：http://nws.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lzj.bjfxy.top

[R17] 数组定义与取值
来源：http://rzk.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vyb.yj20258.top

[R18] 遍历数组
来源：http://mvz.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://csn.daxiang520.top

[R19] 数组长度
来源：http://mhw.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://dua.gotoacloud.top

[R20] 关联数组（字典）
来源：http://vht.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vjr.fktsv.cn

[R21] 字符串长度
来源：http://tkv.wangdashe.top

echo "${#s}"
来源：http://oda.zhaomingkeji.xyz

[R22] 截取子串
来源：http://ivs.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://jfp.zhengqikj.top

[R23] 字符串替换
来源：http://ogs.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fmr.gotoacloud.top

[R24] 大小写转换
来源：http://ovx.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://lyh.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://iad.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gxb.jinqigfzy.top

[R26] 命令替换
来源：http://fva.pengpengdd.cyou

now=$(date +%F); echo "$now"
来源：http://zmb.aibaodan.cn

[R27] 算术展开
来源：http://drz.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://mbs.zdqjudy.top

[R28] 浮点运算
来源：http://uul.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://zfc.cqqwz.cn

[R29] 定义函数
来源：http://urx.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lsg.sxryk.cn

[R30] 函数返回状态码
来源：http://yfs.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://fwo.chenzaomai.com

[R31] 局部变量
来源：http://xtd.hfpthk.cn

f() { local x=1; echo "$x"; }
来源：http://rrk.9152youxi.cn

[R32] 参数个数校验
来源：http://jsc.tanke756.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sxn.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://tut.cucudq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dod.dashuyun.cn

[R34] 退出时清理
来源：http://zsz.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://idr.316326.xyz

[R35] 后台执行并等待
来源：http://wwq.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://enl.haohaochexian.top

[R36] 并发执行多个任务
来源：http://oft.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cxp.cashguo.top

[R37] 把输出赋给变量
来源：http://adm.smart0.xyz

files=$(ls -1)
来源：http://sqj.daxiang520.top

[R38] 管道串联
来源：http://erp.tanke756.top

cat a.txt | grep -i error | wc -l
来源：http://xqe.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://nhh.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://uju.ppjwa.cn

[R40] 追加写日志
来源：http://chh.tian-w.cn

echo "log" >> out.log
来源：http://eau.nanxuanxn.top

[R41] 丢弃输出
来源：http://qqx.shanyushiyangkeji.top

cmd >/dev/null 2>&1
来源：http://wah.yfazqb.com

[R42] 输入重定向
来源：http://svg.snrcjt.cn

wc -l < a.txt
来源：http://lux.nanxinkj.top

[R43] 按名字查找文件
来源：http://xec.sxryk.cn

find . -name "*.log" -type f
来源：http://qdv.bjfxy.top

[R44] 按修改时间查找
来源：http://onf.jlsjyb.cn

find . -mtime -7 -type f
来源：http://scn.snrcjt.cn

[R45] 批量删除
来源：http://ifo.chenjidiqi.icu

find . -name "*.tmp" -delete
来源：http://xkf.xinyue.icu

[R46] 递归替换文件内容
来源：http://uyp.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zaa.jinqigufen.top

[R47] sed 单行替换
来源：http://jeb.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xxv.hywenlv.cn

[R48] awk 取指定列
来源：http://juw.redwolf501.top

awk '{print $1, $3}' a.txt
来源：http://kyp.wangshuangyany.cn

[R49] awk 带条件
来源：http://rzv.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://opo.vqdsnc.cn

[R50] awk 求和
来源：http://dkf.chenlongwang.top

awk '{s += $2} END {print s}' a.txt
来源：http://lhq.birdmap.top

[R51] 排序去重取前几
来源：http://rye.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://spn.nanxinkj.top

[R52] 统计行数
来源：http://eac.guannengcc.top

wc -l a.txt
来源：http://cvr.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://vcv.c1oappe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sfo.jiagoushi.top

[R54] 比较两个文件
来源：http://exa.yvedp.cn

diff a.txt b.txt
来源：http://xhs.yj20258.top

[R55] 压缩与解压
来源：http://rhf.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://clk.redwolf501.top

[R56] 远程拷贝
来源：http://wzl.haohaochexian.top

scp file user@host:/path/
来源：http://fcz.sxryk.cn

[R57] 远程执行命令
来源：http://rof.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://wif.sxryk.cn

[R58] 下载文件
来源：http://qvv.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fpg.cdnleiting.top

[R59] 发 POST JSON
来源：http://thh.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jpg.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://vpf.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qxi.chenzaomai.com

[R61] 磁盘占用
来源：http://ymt.havefunace.top

df -h;  du -sh *
来源：http://mbr.shuidangran.top

[R62] 找最占空间的文件
来源：http://olr.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://vcs.hywenlv.cn

[R63] 内存与进程
来源：http://spi.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://wpa.svipenyu.cn

[R64] 结束进程
来源：http://zyn.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://vfv.daxiang520.top

[R65] 查看端口占用
来源：http://ssb.yj20258888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xdn.jyoumei.cn

[R66] 定时任务
来源：http://bmw.fehbvm.com

crontab -e;  crontab -l
来源：http://vfe.zhiwuduotai.top

[R67] 生成随机十六进制串
来源：http://ygu.kuanghao11.cn

openssl rand -hex 16
来源：http://bkm.cucudq.cn

[R68] 计算文件校验值
来源：http://okg.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://ieb.nanxuanxn.top

[R69] 生成随机密码
来源：http://ngi.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://lfx.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://dso.hfpthk.cn

date +%s;  date -d @1700000000
来源：http://wll.chenlongwang.top

[R71] 日期格式化
来源：http://dru.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wyq.cheryme.top

[R72] 等待端口就绪
来源：http://hhp.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iac.epnwcf.com

[R73] 分割大日志
来源：http://vyl.ctjpmb.com

split -l 1000 big.log part_
来源：http://vqr.yanxiufei.cn

[R74] 批量重命名
来源：http://tkj.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ugm.xuetiantiany.cn

[R75] 导出环境变量
来源：http://lpi.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://dvz.sxryk.cn

[R76] 使用临时文件
来源：http://hox.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cfp.daria6918.cn

[R77] 读取用户输入
来源：http://pdd.hnqzz.top

read -rp "请输入: " ans
来源：http://pyu.jianghu66.top

[R78] 交互式菜单
来源：http://szd.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vko.sjlbkw.cn

[R79] 解析命令行选项
来源：http://hhi.sjlbkw.cn


<!-- 参考信息 -->