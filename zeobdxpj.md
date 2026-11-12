代发 wailian999

[Q33] 多列分组
来源：http://suq.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cqo.ybcxt.top

[Q34] 每组取第一条
来源：http://mjh.52xcode.cn

SELECT * FROM (
来源：http://oqx.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dab.yuanzhike.top

) t WHERE rn = 1;
来源：http://wnl.kuanghao11.cn

[Q35] 内连接
来源：http://rux.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aij.vehdjk.com

[Q36] 左连接
来源：http://vcz.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://msc.316326.xyz

[Q37] 右连接
来源：http://rru.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hyw.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://dbs.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xsa.yfazqb.com

[Q39] 自连接（查上下级）
来源：http://yoc.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sfu.sweek.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ksi.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gpe.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cxk.fzhhl.top

[Q41] 多表连接
来源：http://ukc.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tqs.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://zms.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://wnj.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://mxt.316326.xyz

SELECT u.name, o.amount FROM users u
来源：http://osm.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://upb.yuanzhike.top

[Q43] 标量子查询
来源：http://hrh.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ybp.meibo888.top

[Q44] IN 子查询
来源：http://kvb.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lbc.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://qoa.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://haf.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://sxe.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wbg.xuanzx.com

[Q47] 与平均值比较
来源：http://bog.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tsd.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://ygk.ydjk.org.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hpx.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://cka.hesvh.cn

[Q49] 更新单行
来源：http://eph.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kmb.yj20258888.top

[Q50] 批量更新
来源：http://mig.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ibm.epnwcf.com

[Q51] 用子查询更新
来源：http://war.nanxinkj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hrq.hfpthk.cn

[Q52] 删除指定行
来源：http://fmd.yuxming.cn

DELETE FROM users WHERE id = 10;
来源：http://vno.sxryk.cn

[Q53] 按条件删除
来源：http://xcc.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://puq.chenlongwang.top

[Q54] 清空表
来源：http://nmo.jinqigufen.top

TRUNCATE TABLE logs;
来源：http://ygx.dianchejie.cn

[Q55] 排名（并列占位）
来源：http://jug.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hum.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://fiw.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://exm.svipenyu.cn

[Q57] 行号
来源：http://zpm.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://axo.0kj1m.cn

[Q58] 累计求和
来源：http://zgb.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mtk.hongshengwenyu.top

[Q59] 分组内累计
来源：http://sfm.pengpengdd.cyou

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zff.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://rnr.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fjl.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ywp.yj20258.top

[Q61] 移动平均
来源：http://tbt.wangshuangyany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aae.9152youxi.cn

[Q62] 分组占比
来源：http://ajf.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zsp.tarul.cn

[Q63] 开启事务
来源：http://nvr.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://iss.nanxuanxn.top

[Q64] 提交事务
来源：http://vks.feifeiyinyue.top

COMMIT;
来源：http://evx.xinyue.icu

[Q65] 回滚事务
来源：http://hcl.ctjpmb.com

ROLLBACK;
来源：http://rmr.zdbjq.cn

[Q66] 行锁查询
来源：http://zia.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://taa.aizwys.cn

[Q67] 设置隔离级别
来源：http://vbw.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fjy.jinyuanbaomall.cn

[Q68] 保存点
来源：http://eoz.kuanghao11.cn

SAVEPOINT sp1;
来源：http://crv.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://vvf.bbcook.cn

[Q69] 查看执行计划
来源：http://hgv.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pmi.cqqwz.cn

[Q70] 更新统计信息
来源：http://xiz.xylfe.cn

ANALYZE TABLE users;
来源：http://ytu.yuanzhike.top

[Q71] 查看建表语句
来源：http://zcp.dashuyun.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iel.fzhhl.top

[Q72] 查看索引
来源：http://qsb.zhengqikj.top

SHOW INDEX FROM users;
来源：http://cyn.9152youxi.cn

[Q73] 查看表状态
来源：http://zav.vehdjk.com

SHOW TABLE STATUS LIKE 'users';
来源：http://yxa.shzxlz.cn

[Q74] 强制使用索引
来源：http://ihk.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zac.yj20258.top

[Q75] 日期格式化
来源：http://som.zhiwuduotai.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://beo.xylfe.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wsl.andypj.xyz

[Q76] 按天统计
来源：http://fuo.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nhy.hywenlv.cn

[Q77] 时间加减
来源：http://stm.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uxm.zhiwuduotai.top

[Q78] 当前时间
来源：http://qkg.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qpv.hysaishi.cn

[Q79] 字符串拼接
来源：http://kzm.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jxk.haohaochexian.top

[Q80] 字符串截取
来源：http://ikw.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yxk.nanxinkj.top

[Q81] 字符串替换
来源：http://ulf.havefunace.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qoi.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://xyu.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dut.gogol.net.cn

[Q83] 大小写转换
来源：http://vuo.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xqj.jyoumei.cn

[Q84] 去除首尾空格
来源：http://drk.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://tup.fzhhl.top

[Q85] 数值取整
来源：http://emw.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yjk.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://swf.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uxx.redwolf501.top

[Q87] JSON 字段做条件
来源：http://jpv.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iya.sweek.top

[Q88] 行转列（条件聚合）
来源：http://oue.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mwm.redwolf501.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gpf.ydzc1.top

[Q89] 判断表是否存在
来源：http://flu.ydjk.org.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yst.xziqi.cn

[Q90] 生成序号列
来源：http://wui.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mcj.nwbrower.top

================================================================================
来源：http://vnz.guannengcc.top

R. Bash 专题
来源：http://aul.ivvv.top

================================================================================
来源：http://kwx.hfpthk.cn

[R01] shebang 与严格模式
来源：http://bpm.yj20258888.top

#!/usr/bin/env bash
来源：http://ihb.hywenlv.cn

set -euo pipefail
来源：http://pht.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://xks.sweek.top

name="Tom"; echo "$name"
来源：http://fle.hfpthk.cn

[R03] 只读变量
来源：http://oqd.cheryme.top

readonly PI=3.14
来源：http://ler.vehdjk.com

[R04] 位置参数
来源：http://vod.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qqd.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://are.dianchejie.cn

name="${1:-default}"
来源：http://cje.shuidangran.top

[R06] 判断命令是否存在
来源：http://rnj.ctjpmb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://voy.iojbl.cn

[R07] if 判断文件
来源：http://oaq.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ias.yj20258.top

[R08] 数值比较
来源：http://grq.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dnz.sweek.top

[R09] 字符串比较
来源：http://wjw.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fmb.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://yyb.snrcjt.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pxl.andypj.xyz

[R11] case 多分支
来源：http://drv.52xcode.cn

case "$1" in
来源：http://nsa.gogol.net.cn

start) echo "启动" ;;
来源：http://ytn.jqgfzy.top

stop)  echo "停止" ;;
来源：http://uxa.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://rfh.nanxuanxn.top

esac
来源：http://guy.snrcjt.cn

[R12] for 遍历文件
来源：http://ncp.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://rri.bbcook.cn

[R13] for 计数循环
来源：http://oea.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://gxv.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://snp.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wog.hesvh.cn

[R15] while 逐行读文件
来源：http://kmz.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vxz.shanyushiyangtech.top

[R16] until 等待条件
来源：http://rng.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fis.mhx1999.top

[R17] 数组定义与取值
来源：http://vcp.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://ptt.c1oappe.top

[R18] 遍历数组
来源：http://ghi.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uvu.jianghu66.top

[R19] 数组长度
来源：http://yzc.hcnkem.com

echo "${#arr[@]}"
来源：http://bga.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://eir.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hub.xziqi.cn

[R21] 字符串长度
来源：http://ypj.cucudq.cn

echo "${#s}"
来源：http://qth.dashuyun.cn

[R22] 截取子串
来源：http://ybw.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://mdw.cashguo.top

[R23] 字符串替换
来源：http://ybt.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blp.jinghuilouyu.cn

[R24] 大小写转换
来源：http://xkt.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://yie.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://pqm.zycfv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lsg.daxiang520.top

[R26] 命令替换
来源：http://ltd.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://mze.zhiwuduotai.top

[R27] 算术展开
来源：http://jyf.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://xya.zhongyouzk.top

[R28] 浮点运算
来源：http://nat.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://wtz.bbcook.cn

[R29] 定义函数
来源：http://ukd.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gbl.yvedp.cn

[R30] 函数返回状态码
来源：http://eme.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://enc.gzhubu.top

[R31] 局部变量
来源：http://ekr.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://vsb.xinyue.icu

[R32] 参数个数校验
来源：http://mif.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tgc.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://jrl.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vza.nanxuanxn.top

[R34] 退出时清理
来源：http://ifm.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rmp.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://wes.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mog.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://emi.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eoc.zycfv.cn

[R37] 把输出赋给变量
来源：http://ypq.mhx1999.top

files=$(ls -1)
来源：http://taq.xylfe.cn

[R38] 管道串联
来源：http://zec.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://fbe.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://hxb.c1oappe.top

cmd > out.log 2>&1
来源：http://zll.9152youxi.cn

[R40] 追加写日志
来源：http://blr.wangdashe.top

echo "log" >> out.log
来源：http://fdz.yj202588.top

[R41] 丢弃输出
来源：http://hde.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://cml.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://ofc.cashguo.top

wc -l < a.txt
来源：http://vnm.pycfn.com

[R43] 按名字查找文件
来源：http://lmh.jiagoushi.top

find . -name "*.log" -type f
来源：http://bpx.sjlbkw.cn

[R44] 按修改时间查找
来源：http://nyk.cucudq.cn

find . -mtime -7 -type f
来源：http://sgr.hcnkem.com

[R45] 批量删除
来源：http://luf.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://dyu.ydzc1.top

[R46] 递归替换文件内容
来源：http://evb.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ruu.ybcxt.top

[R47] sed 单行替换
来源：http://zxt.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://ojs.cqqwz.cn

[R48] awk 取指定列
来源：http://nzz.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://qmx.snrcjt.cn

[R49] awk 带条件
来源：http://jme.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qxu.yj20258.top

[R50] awk 求和
来源：http://ewd.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fao.c1oappe.top

[R51] 排序去重取前几
来源：http://nru.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://aqt.hfpthk.cn

[R52] 统计行数
来源：http://usc.bjfxy.top

wc -l a.txt
来源：http://rhx.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://mcy.jinghuilouyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vvx.yuxming.cn

[R54] 比较两个文件
来源：http://urg.wangshuangyany.cn

diff a.txt b.txt
来源：http://nuo.hesvh.cn

[R55] 压缩与解压
来源：http://ntl.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tlo.9152youxi.cn

[R56] 远程拷贝
来源：http://fsb.jianghu66.top

scp file user@host:/path/
来源：http://jub.0kj1m.cn

[R57] 远程执行命令
来源：http://jom.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://uto.52xcode.cn

[R58] 下载文件
来源：http://rzu.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://brx.tarul.cn

[R59] 发 POST JSON
来源：http://zng.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vmw.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://tqn.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://whr.bjfxy.top

[R61] 磁盘占用
来源：http://qfb.guannengcc.top

df -h;  du -sh *
来源：http://sgq.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://ags.birdmap.top

du -ah . | sort -rh | head -10
来源：http://slw.quarkkingdee.top

[R63] 内存与进程
来源：http://qkk.fzhhl.top

free -h;  ps aux | grep nginx
来源：http://tgs.ydjk.org.cn

[R64] 结束进程
来源：http://koq.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://wwq.9152youxi.cn

[R65] 查看端口占用
来源：http://prq.xingfuxueyuan.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tth.yuanzhike.top

[R66] 定时任务
来源：http://vtx.yfazqb.com

crontab -e;  crontab -l
来源：http://mqg.bjfxy.top

[R67] 生成随机十六进制串
来源：http://yke.xuetiantiany.cn

openssl rand -hex 16
来源：http://rrh.pengpengdd.cyou

[R68] 计算文件校验值
来源：http://lsb.ivvv.top

sha256sum a.txt;  md5sum a.txt
来源：http://slf.fktsv.cn

[R69] 生成随机密码
来源：http://jvf.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://qpo.vqdsnc.cn

[R70] 时间戳与互转
来源：http://znk.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://qbc.dashuyun.cn

[R71] 日期格式化
来源：http://cbp.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://wez.tanke756.top

[R72] 等待端口就绪
来源：http://ikg.ydjk.org.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cnz.jinqigufen.top

[R73] 分割大日志
来源：http://mqp.jlsjyb.cn

split -l 1000 big.log part_
来源：http://nei.smart0.xyz

[R74] 批量重命名
来源：http://ign.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://suh.nanxuanxn.top

[R75] 导出环境变量
来源：http://hgk.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://xwq.aizwys.cn

[R76] 使用临时文件
来源：http://lcx.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dut.yuanzhike.top

[R77] 读取用户输入
来源：http://rze.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://pns.hfpthk.cn

[R78] 交互式菜单
来源：http://beo.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rcd.xylfe.cn

[R79] 解析命令行选项
来源：http://sdp.ivvv.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ddo.uphjek.com

[R80] 查看脚本执行耗时
来源：http://grm.chenlongwang.top

time ./run.sh
来源：http://ffa.zhijiandao.cn

================================================================================
来源：http://beq.svipenyu.cn

S. C / C++ 专题
来源：http://uqu.cqqwz.cn

================================================================================
来源：http://gkd.xziqi.cn

[S01] C：Hello World
来源：http://zbt.yonumen.top

#include <stdio.h>
来源：http://jrf.hnxiangtu.top


<!-- 参考信息 -->