代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bte.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://jkh.gzhubu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aqv.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://emp.yj202588.top

[Q33] 多列分组
来源：http://ojt.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tjs.epnwcf.com

[Q34] 每组取第一条
来源：http://ffx.bjfxy.top

SELECT * FROM (
来源：http://xcf.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://box.wangdashe.top

) t WHERE rn = 1;
来源：http://uzg.guowangkeji.top

[Q35] 内连接
来源：http://mat.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kjj.redwolf501.top

[Q36] 左连接
来源：http://bgo.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://neg.bjfxy.top

[Q37] 右连接
来源：http://pdl.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gcs.gogol.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sqz.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zyf.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://zox.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nfd.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wnw.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ibt.mhx1999.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bmo.fktsv.cn

[Q41] 多表连接
来源：http://dwt.gzhubu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://amh.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://pce.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://azi.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://vwb.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://esc.havefunace.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eqb.jqgufenzy.top

[Q43] 标量子查询
来源：http://mii.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uvo.0kj1m.cn

[Q44] IN 子查询
来源：http://agg.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yco.ywan-chungtsiang.top

[Q45] EXISTS 判断存在
来源：http://gkg.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rgm.fengsongda.top

[Q46] NOT EXISTS 判断不存在
来源：http://mig.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xeb.ydjk.org.cn

[Q47] 与平均值比较
来源：http://qab.ivvv.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bim.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://xhd.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://idz.chenjidiqi.icu

SELECT * FROM t WHERE c > 5;
来源：http://bae.xinyue.icu

[Q49] 更新单行
来源：http://aax.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ppr.yangfankeji.com

[Q50] 批量更新
来源：http://nii.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zur.yanxiufei.cn

[Q51] 用子查询更新
来源：http://dgg.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iel.fengsongda.top

[Q52] 删除指定行
来源：http://qxo.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://dtw.ppjwa.cn

[Q53] 按条件删除
来源：http://bda.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dqe.shuidangran.top

[Q54] 清空表
来源：http://cmf.hesvh.cn

TRUNCATE TABLE logs;
来源：http://wsq.cucudq.cn

[Q55] 排名（并列占位）
来源：http://mpb.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jvz.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://ywi.nanxuanxn.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dkv.guowangkeji.top

[Q57] 行号
来源：http://yhc.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://opv.bjfxy.top

[Q58] 累计求和
来源：http://end.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vgc.hesvh.cn

[Q59] 分组内累计
来源：http://rek.xingfuxueyuan.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dex.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://rhv.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aft.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yxg.jyoumei.cn

[Q61] 移动平均
来源：http://hnk.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://imx.sjlbkw.cn

[Q62] 分组占比
来源：http://tus.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ibs.zhaomingkeji.xyz

[Q63] 开启事务
来源：http://cux.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://lal.gzhubu.top

[Q64] 提交事务
来源：http://xqe.smart0.xyz

COMMIT;
来源：http://qoa.zhixingplan.top

[Q65] 回滚事务
来源：http://ujj.uphjek.com

ROLLBACK;
来源：http://nbq.0kj1m.cn

[Q66] 行锁查询
来源：http://ivi.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rdb.hammf.cn

[Q67] 设置隔离级别
来源：http://bxt.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ftv.yanxiufei.cn

[Q68] 保存点
来源：http://nnn.sweek.top

SAVEPOINT sp1;
来源：http://hgg.cheryme.top

ROLLBACK TO sp1;
来源：http://vsb.jqgufenzy.top

[Q69] 查看执行计划
来源：http://rof.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ejd.svipenyu.cn

[Q70] 更新统计信息
来源：http://cjd.yanxiufei.cn

ANALYZE TABLE users;
来源：http://zfd.tanke756.top

[Q71] 查看建表语句
来源：http://ada.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wuz.yangfankeji.com

[Q72] 查看索引
来源：http://qnr.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://gvp.hysaishi.cn

[Q73] 查看表状态
来源：http://wry.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ebs.jinyuanbaomall.cn

[Q74] 强制使用索引
来源：http://den.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://usc.jqgfzy.top

[Q75] 日期格式化
来源：http://mlh.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xgz.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vzy.nanxuanxn.top

[Q76] 按天统计
来源：http://ddv.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://axs.jqgfzy.top

[Q77] 时间加减
来源：http://fkz.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rcn.sysykeji.top

[Q78] 当前时间
来源：http://pbg.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yjn.zycfv.cn

[Q79] 字符串拼接
来源：http://ayr.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hfr.daxiang520.top

[Q80] 字符串截取
来源：http://pnj.hnxiangtu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hjo.ppjwa.cn

[Q81] 字符串替换
来源：http://fjs.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lcm.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://wkn.zhongyouzk.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gav.nwbrower.top

[Q83] 大小写转换
来源：http://ufw.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eop.chenlongwang.top

[Q84] 去除首尾空格
来源：http://ads.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://ucr.hysaishi.cn

[Q85] 数值取整
来源：http://wrw.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jvq.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://kkh.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://agj.fanxiaobao.xyz

[Q87] JSON 字段做条件
来源：http://hci.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bjp.birdmap.top

[Q88] 行转列（条件聚合）
来源：http://xvj.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://drv.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xth.yvedp.cn

[Q89] 判断表是否存在
来源：http://wsb.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sua.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://ibn.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zxy.vqdsnc.cn

================================================================================
来源：http://bxs.9152youxi.cn

R. Bash 专题
来源：http://jvz.svipenyu.cn

================================================================================
来源：http://lia.dianchejie.cn

[R01] shebang 与严格模式
来源：http://saz.sxryk.cn

#!/usr/bin/env bash
来源：http://uxz.yuanzhike.top

set -euo pipefail
来源：http://ruj.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://phi.xinyue.icu

name="Tom"; echo "$name"
来源：http://llx.yanxiufei.cn

[R03] 只读变量
来源：http://mls.xinyue.icu

readonly PI=3.14
来源：http://mzq.yvedp.cn

[R04] 位置参数
来源：http://jvz.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fbp.zhijiandao.cn

[R05] 参数默认值
来源：http://cni.tanke756.top

name="${1:-default}"
来源：http://gxk.sysykeji.top

[R06] 判断命令是否存在
来源：http://enz.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://klm.ctjpmb.com

[R07] if 判断文件
来源：http://ipo.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://diu.feifeiyinyue.top

[R08] 数值比较
来源：http://qqu.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pwf.316326.xyz

[R09] 字符串比较
来源：http://fpt.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vni.cqqwz.cn

[R10] 正则匹配
来源：http://sep.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://shg.birdmap.top

[R11] case 多分支
来源：http://lwc.meibo888.top

case "$1" in
来源：http://qbc.yonumen.top

start) echo "启动" ;;
来源：http://csk.hywenlv.cn

stop)  echo "停止" ;;
来源：http://uan.xinyue.icu

*)     echo "未知命令" ;;
来源：http://bmv.yangfankeji.com

esac
来源：http://pbp.havefunace.top

[R12] for 遍历文件
来源：http://ekd.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://vku.quarkkingdee.top

[R13] for 计数循环
来源：http://niy.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://equ.aibaodan.cn

[R14] C 风格 for
来源：http://eup.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://swo.gotoacloud.top

[R15] while 逐行读文件
来源：http://tni.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cmq.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://xqp.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sjf.zdqjudy.top

[R17] 数组定义与取值
来源：http://rkj.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://lhp.vqdsnc.cn

[R18] 遍历数组
来源：http://egg.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uie.bbcook.cn

[R19] 数组长度
来源：http://vvc.nanxuanxn.top

echo "${#arr[@]}"
来源：http://cwa.guowangkeji.top

[R20] 关联数组（字典）
来源：http://gul.havefunace.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bxw.nwbrower.top

[R21] 字符串长度
来源：http://vej.zhiwuduotai.top

echo "${#s}"
来源：http://lec.shuidangran.top

[R22] 截取子串
来源：http://zfz.feifeiyinyue.top

echo "${s:0:5}"
来源：http://fbm.cheryme.top

[R23] 字符串替换
来源：http://zcb.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bgl.jianghu66.top

[R24] 大小写转换
来源：http://xlb.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://xpf.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://afr.yanxiufei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ols.kuanghao11.cn

[R26] 命令替换
来源：http://xol.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://aiq.fanxiaobao.xyz

[R27] 算术展开
来源：http://xxt.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://jdl.hnqzz.top

[R28] 浮点运算
来源：http://iie.yj20258888.top

echo "scale=2; 10/3" | bc
来源：http://vde.yj20258888.top

[R29] 定义函数
来源：http://rfc.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gaz.bbcook.cn

[R30] 函数返回状态码
来源：http://eaq.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://gok.wangdashe.top

[R31] 局部变量
来源：http://hrc.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://jqq.yueranfly.top

[R32] 参数个数校验
来源：http://dkw.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rop.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://akh.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rsg.yj20258.top

[R34] 退出时清理
来源：http://euc.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://kgz.hnxiangtu.top

[R35] 后台执行并等待
来源：http://mxd.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pfv.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://ymi.daria6918.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jzy.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://hib.wangdashe.top

files=$(ls -1)
来源：http://bza.guowangkeji.top

[R38] 管道串联
来源：http://teu.yvedp.cn

cat a.txt | grep -i error | wc -l
来源：http://bnd.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://wrh.52xcode.cn

cmd > out.log 2>&1
来源：http://djq.dashuyun.cn

[R40] 追加写日志
来源：http://mhn.havefunace.top

echo "log" >> out.log
来源：http://msu.shangyingyoupin.top

[R41] 丢弃输出
来源：http://vcb.mhx1999.top

cmd >/dev/null 2>&1
来源：http://ltv.ivvv.top

[R42] 输入重定向
来源：http://fpq.ivvv.top

wc -l < a.txt
来源：http://ysz.chenzaomai.com

[R43] 按名字查找文件
来源：http://lyp.shzxlz.cn

find . -name "*.log" -type f
来源：http://pox.hnxiangtu.top

[R44] 按修改时间查找
来源：http://zso.c1oappe.top

find . -mtime -7 -type f
来源：http://gdo.0kj1m.cn

[R45] 批量删除
来源：http://eil.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://rra.hnqzz.top

[R46] 递归替换文件内容
来源：http://qkx.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uzz.shzxlz.cn

[R47] sed 单行替换
来源：http://ykq.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://ezw.chenzaomai.com

[R48] awk 取指定列
来源：http://sjk.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://iao.xuetiantiany.cn

[R49] awk 带条件
来源：http://oyf.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aag.yj202588.top

[R50] awk 求和
来源：http://yye.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://hrt.yonumen.top

[R51] 排序去重取前几
来源：http://zbp.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://oce.vqdsnc.cn

[R52] 统计行数
来源：http://nvp.gzhubu.top

wc -l a.txt
来源：http://ujr.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://rvr.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kdi.mhx1999.top

[R54] 比较两个文件
来源：http://njw.mhx1999.top

diff a.txt b.txt
来源：http://yhk.fehbvm.com

[R55] 压缩与解压
来源：http://nhg.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dmc.guowangkeji.top

[R56] 远程拷贝
来源：http://cnd.cdnleiting.top

scp file user@host:/path/
来源：http://iso.wangdashe.top

[R57] 远程执行命令
来源：http://hdm.gogol.net.cn

ssh user@host 'uptime'
来源：http://evf.fanxiaobao.xyz

[R58] 下载文件
来源：http://tgk.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hqz.cashguo.top

[R59] 发 POST JSON
来源：http://qxg.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xcz.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://rgw.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jew.chenzaomai.com

[R61] 磁盘占用
来源：http://nvo.jinghuilouyu.cn

df -h;  du -sh *
来源：http://zqt.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://srm.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://ows.guowangkeji.top

[R63] 内存与进程
来源：http://tzi.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://joc.hesvh.cn

[R64] 结束进程
来源：http://gfq.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://mch.ehwqpu.com

[R65] 查看端口占用
来源：http://yqi.zhiwuduotai.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wty.feifeiyinyue.top

[R66] 定时任务
来源：http://zam.ctjpmb.com

crontab -e;  crontab -l
来源：http://khj.daria6918.cn

[R67] 生成随机十六进制串
来源：http://non.zhongyouzk.top

openssl rand -hex 16
来源：http://ycb.yangfankeji.com

[R68] 计算文件校验值
来源：http://mwk.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://eyv.xziqi.cn

[R69] 生成随机密码
来源：http://amu.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://lad.gzhubu.top

[R70] 时间戳与互转
来源：http://xgd.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://ncn.sysykeji.top

[R71] 日期格式化
来源：http://cxr.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kxi.ivvv.top

[R72] 等待端口就绪
来源：http://jbg.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nnb.havefunace.top

[R73] 分割大日志
来源：http://xbj.fktsv.cn

split -l 1000 big.log part_
来源：http://utd.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://gae.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ydf.pengpengdd.cyou

[R75] 导出环境变量
来源：http://iwr.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://mls.hcnkem.com

[R76] 使用临时文件
来源：http://era.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xcu.shuidangran.top

[R77] 读取用户输入
来源：http://kaz.sxryk.cn

read -rp "请输入: " ans
来源：http://tvv.fktsv.cn

[R78] 交互式菜单
来源：http://avb.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://qrs.sysykeji.top

[R79] 解析命令行选项
来源：http://epx.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://crm.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://gup.sweek.top

time ./run.sh
来源：http://bzz.aizwys.cn

================================================================================
来源：http://kqt.svipenyu.cn


<!-- 参考信息 -->