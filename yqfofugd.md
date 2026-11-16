代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fzg.hcnkem.com

) t WHERE rn = 1;
来源：http://qdp.ehwqpu.com

[Q35] 内连接
来源：http://wrj.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mie.yonumen.top

[Q36] 左连接
来源：http://guw.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mno.yonumen.top

[Q37] 右连接
来源：http://ssl.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ezq.sysykeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://lpc.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://njl.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://ons.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ldf.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pzm.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zot.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jwo.cheryme.top

[Q41] 多表连接
来源：http://zqu.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cnj.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://qft.xuanzx.com

JOIN products p ON p.id = o.product_id;
来源：http://bdd.guannengcc.top

[Q42] 连接条件附加过滤
来源：http://qex.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://nep.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yxp.cucudq.cn

[Q43] 标量子查询
来源：http://qgp.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ajo.shzxlz.cn

[Q44] IN 子查询
来源：http://kfe.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vwx.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://ifa.cashguo.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://but.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xga.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jju.chenlongwang.top

[Q47] 与平均值比较
来源：http://hcu.zhijiandao.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ycg.tarul.cn

[Q48] CTE 公用表表达式
来源：http://zyi.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://thw.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://vis.daria6918.cn

[Q49] 更新单行
来源：http://tut.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mxt.chenzaomai.com

[Q50] 批量更新
来源：http://zwn.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dyz.tarul.cn

[Q51] 用子查询更新
来源：http://jpj.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jfl.yueranfly.top

[Q52] 删除指定行
来源：http://ngd.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://pkw.yuanzhike.top

[Q53] 按条件删除
来源：http://elm.yvedp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ebb.bjfxy.top

[Q54] 清空表
来源：http://pnq.gaohongyu789.top

TRUNCATE TABLE logs;
来源：http://xjs.jianghu66.top

[Q55] 排名（并列占位）
来源：http://jli.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ddf.jianghu66.top

[Q56] 密集排名（并列不占位）
来源：http://dbq.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hwj.jinyuanbaomall.cn

[Q57] 行号
来源：http://vjy.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vlq.zhiwuduotai.top

[Q58] 累计求和
来源：http://pqy.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vtu.tanke756.top

[Q59] 分组内累计
来源：http://vub.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sfn.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://cic.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uji.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cib.yueranfly.top

[Q61] 移动平均
来源：http://typ.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vck.bjfxy.top

[Q62] 分组占比
来源：http://iix.jlsjyb.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fkv.shuidangran.top

[Q63] 开启事务
来源：http://hup.shzxlz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://iif.zhaomingkeji.xyz

[Q64] 提交事务
来源：http://wau.wangdashe.top

COMMIT;
来源：http://ibp.svipenyu.cn

[Q65] 回滚事务
来源：http://gnq.fengsongda.top

ROLLBACK;
来源：http://mna.daxiang520.top

[Q66] 行锁查询
来源：http://hbr.ydjk.org.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://civ.zhaomingkeji.xyz

[Q67] 设置隔离级别
来源：http://nuq.52xcode.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://woc.gzhubu.top

[Q68] 保存点
来源：http://mht.yj20258888.top

SAVEPOINT sp1;
来源：http://ska.shuidangran.top

ROLLBACK TO sp1;
来源：http://xjn.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://eub.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mhd.nanxinkj.top

[Q70] 更新统计信息
来源：http://xus.jlsjyb.cn

ANALYZE TABLE users;
来源：http://bef.zdbjq.cn

[Q71] 查看建表语句
来源：http://mxn.dashuyun.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tsx.daria6918.cn

[Q72] 查看索引
来源：http://boq.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://bsn.xuanzx.com

[Q73] 查看表状态
来源：http://kkj.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://epi.yongpay.top

[Q74] 强制使用索引
来源：http://mtl.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jdc.gaohongyu789.top

[Q75] 日期格式化
来源：http://cdt.yuanzhike.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://afq.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cmt.ppjwa.cn

[Q76] 按天统计
来源：http://nbl.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uxr.wangshuangyany.cn

[Q77] 时间加减
来源：http://yke.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pzv.xuanzx.com

[Q78] 当前时间
来源：http://hpi.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kuj.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://yaz.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ccv.cdnleiting.top

[Q80] 字符串截取
来源：http://sdb.shanyushiyangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ugq.jianghu66.top

[Q81] 字符串替换
来源：http://jak.bjfxy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fne.dianchejie.cn

[Q82] 字符长度与字节长度
来源：http://wus.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zjd.cucudq.cn

[Q83] 大小写转换
来源：http://jmt.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://odv.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://twn.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://qtw.cheryme.top

[Q85] 数值取整
来源：http://vwz.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://swk.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://enn.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jer.pycfn.com

[Q87] JSON 字段做条件
来源：http://nbo.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zfh.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://nch.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cfd.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tzw.havefunace.top

[Q89] 判断表是否存在
来源：http://yql.mhx1999.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pkj.gotoacloud.top

[Q90] 生成序号列
来源：http://prq.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cyv.svipenyu.cn

================================================================================
来源：http://itb.ywan-chungtsiang.top

R. Bash 专题
来源：http://amm.wangshuangyany.cn

================================================================================
来源：http://xgp.316326.xyz

[R01] shebang 与严格模式
来源：http://rxv.c1oappe.top

#!/usr/bin/env bash
来源：http://pkn.hnxiangtu.top

set -euo pipefail
来源：http://fyd.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://orc.sjlbkw.cn

name="Tom"; echo "$name"
来源：http://jzd.snrcjt.cn

[R03] 只读变量
来源：http://biv.yuanzhike.top

readonly PI=3.14
来源：http://ade.hnqzz.top

[R04] 位置参数
来源：http://maa.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qke.hywenlv.cn

[R05] 参数默认值
来源：http://nut.shangyingyoupin.top

name="${1:-default}"
来源：http://esi.chenjidiqi.icu

[R06] 判断命令是否存在
来源：http://pan.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oae.316326.xyz

[R07] if 判断文件
来源：http://erz.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rvw.hnqzz.top

[R08] 数值比较
来源：http://xkm.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://yyl.xylfe.cn

[R09] 字符串比较
来源：http://oon.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kkr.andypj.xyz

[R10] 正则匹配
来源：http://yqt.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://krn.shangyingyoupin.top

[R11] case 多分支
来源：http://oze.zhaomingkeji.xyz

case "$1" in
来源：http://moq.xylfe.cn

start) echo "启动" ;;
来源：http://wtm.hnqzz.top

stop)  echo "停止" ;;
来源：http://dlx.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://gxd.redwolf501.top

esac
来源：http://iwn.cdnleiting.top

[R12] for 遍历文件
来源：http://jel.bbcook.cn

for f in *.txt; do echo "$f"; done
来源：http://ewf.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://zzh.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://lfu.aibaodan.cn

[R14] C 风格 for
来源：http://grx.yfazqb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://npn.shzxlz.cn

[R15] while 逐行读文件
来源：http://ifd.epnwcf.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dki.ctjpmb.com

[R16] until 等待条件
来源：http://zbn.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zwn.ivvv.top

[R17] 数组定义与取值
来源：http://edi.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://hnx.gzhubu.top

[R18] 遍历数组
来源：http://jze.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gdf.shanyushiyangkeji.top

[R19] 数组长度
来源：http://fjz.jyoumei.cn

echo "${#arr[@]}"
来源：http://yoo.hywenlv.cn

[R20] 关联数组（字典）
来源：http://ary.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rbp.yuxming.cn

[R21] 字符串长度
来源：http://mkl.jinqigfzy.top

echo "${#s}"
来源：http://mmg.jinyuanbaomall.cn

[R22] 截取子串
来源：http://sla.tian-w.cn

echo "${s:0:5}"
来源：http://kea.sjlbkw.cn

[R23] 字符串替换
来源：http://nwx.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bwe.smart0.xyz

[R24] 大小写转换
来源：http://dcp.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ofv.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://wdh.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mmp.hcnkem.com

[R26] 命令替换
来源：http://rwb.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://atv.zhoulong.xyz

[R27] 算术展开
来源：http://qzd.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://hxo.yfazqb.com

[R28] 浮点运算
来源：http://ukm.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://qly.xylfe.cn

[R29] 定义函数
来源：http://csa.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zkw.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://dht.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://nhz.9152youxi.cn

[R31] 局部变量
来源：http://opg.shanyushiyangtech.top

f() { local x=1; echo "$x"; }
来源：http://wsf.yanxiufei.cn

[R32] 参数个数校验
来源：http://cim.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ibm.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://wsb.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gvs.jinqigufen.top

[R34] 退出时清理
来源：http://wpo.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zui.zhixingplan.top

[R35] 后台执行并等待
来源：http://rfl.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://hfr.yj20258.top

[R36] 并发执行多个任务
来源：http://ahd.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dxk.dashuyun.cn

[R37] 把输出赋给变量
来源：http://dzp.wangdashe.top

files=$(ls -1)
来源：http://ohs.aibaodan.cn

[R38] 管道串联
来源：http://wgm.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://wvl.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://bqf.hysaishi.cn

cmd > out.log 2>&1
来源：http://bni.cdnleiting.top

[R40] 追加写日志
来源：http://hmw.tarul.cn

echo "log" >> out.log
来源：http://hua.hammf.cn

[R41] 丢弃输出
来源：http://dbc.tian-w.cn

cmd >/dev/null 2>&1
来源：http://cbk.fzhhl.top

[R42] 输入重定向
来源：http://dnq.yuxming.cn

wc -l < a.txt
来源：http://dpk.9152youxi.cn

[R43] 按名字查找文件
来源：http://sqx.jiagoushi.top

find . -name "*.log" -type f
来源：http://kwy.sysykeji.top

[R44] 按修改时间查找
来源：http://kcy.c1oappe.top

find . -mtime -7 -type f
来源：http://uoh.hongshengwenyu.top

[R45] 批量删除
来源：http://wqc.fengsongda.top

find . -name "*.tmp" -delete
来源：http://riz.sufxvd.cn

[R46] 递归替换文件内容
来源：http://wzf.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wtd.jiagoushi.top

[R47] sed 单行替换
来源：http://zon.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iyj.snrcjt.cn

[R48] awk 取指定列
来源：http://ynk.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://gex.jlsjyb.cn

[R49] awk 带条件
来源：http://ujl.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yrp.zhengqikj.top

[R50] awk 求和
来源：http://dgj.fktsv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nhw.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://bio.wangshuangyany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kqy.316326.xyz

[R52] 统计行数
来源：http://gov.jiagoushi.top

wc -l a.txt
来源：http://uag.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://kjk.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kop.chenzaomai.com

[R54] 比较两个文件
来源：http://lvn.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://hni.nanxinkj.top

[R55] 压缩与解压
来源：http://pgt.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ncg.xylfe.cn

[R56] 远程拷贝
来源：http://hnh.sweek.top

scp file user@host:/path/
来源：http://pue.epnwcf.com

[R57] 远程执行命令
来源：http://zeu.gaohongyu789.top

ssh user@host 'uptime'
来源：http://zvu.hcnkem.com

[R58] 下载文件
来源：http://wga.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vgo.yanxiufei.cn

[R59] 发 POST JSON
来源：http://eso.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uka.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://oih.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bgh.sweek.top

[R61] 磁盘占用
来源：http://adr.pycfn.com

df -h;  du -sh *
来源：http://lbb.xylfe.cn

[R62] 找最占空间的文件
来源：http://ckt.bjfxy.top

du -ah . | sort -rh | head -10
来源：http://ckk.yanxiufei.cn

[R63] 内存与进程
来源：http://pxa.cdnleiting.top

free -h;  ps aux | grep nginx
来源：http://oad.mhx1999.top

[R64] 结束进程
来源：http://moq.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://axe.daxiang520.top

[R65] 查看端口占用
来源：http://cfm.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ykb.hysaishi.cn

[R66] 定时任务
来源：http://vov.sweek.top

crontab -e;  crontab -l
来源：http://thh.xziqi.cn

[R67] 生成随机十六进制串
来源：http://orp.xziqi.cn

openssl rand -hex 16
来源：http://aki.zhengqikj.top

[R68] 计算文件校验值
来源：http://sph.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://tyq.xuanzx.com

[R69] 生成随机密码
来源：http://eod.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://byp.jlsjyb.cn

[R70] 时间戳与互转
来源：http://zrq.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://ipz.bjfxy.top

[R71] 日期格式化
来源：http://zzi.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nzs.gaohongyu789.top

[R72] 等待端口就绪
来源：http://ksx.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://axq.quarkkingdee.top

[R73] 分割大日志
来源：http://nse.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://tnp.kuanghao11.cn

[R74] 批量重命名
来源：http://ecf.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://foq.316326.xyz

[R75] 导出环境变量
来源：http://mxi.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://jlm.sweek.top

[R76] 使用临时文件
来源：http://bge.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zbx.shuidangran.top

[R77] 读取用户输入
来源：http://ipn.iojbl.cn

read -rp "请输入: " ans
来源：http://tgf.dianchejie.cn

[R78] 交互式菜单
来源：http://aip.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ult.hnxiangtu.top

[R79] 解析命令行选项
来源：http://bux.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gnf.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://brs.hesvh.cn

time ./run.sh
来源：http://jgl.svipenyu.cn

================================================================================
来源：http://pao.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://skj.sjlbkw.cn

================================================================================
来源：http://agh.sufxvd.cn

[S01] C：Hello World
来源：http://xcm.fengsongda.top

#include <stdio.h>
来源：http://fhp.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://xzl.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://mia.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://nbu.316326.xyz

[S03] C：读入整数
来源：http://has.ybcxt.top


<!-- 参考信息 -->