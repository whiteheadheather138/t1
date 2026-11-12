代发 wailian999

[Q36] 左连接
来源：http://jmd.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://smo.sjlbkw.cn

[Q37] 右连接
来源：http://mxe.zdbjq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kcn.meibo888.top

[Q38] 全外连接（PostgreSQL）
来源：http://jfu.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gge.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://ens.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://evr.hywenlv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qof.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://usp.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jkh.vehdjk.com

[Q41] 多表连接
来源：http://faf.cucudq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mar.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://mpn.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://ovh.vehdjk.com

[Q42] 连接条件附加过滤
来源：http://bum.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://mqg.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kei.gogol.net.cn

[Q43] 标量子查询
来源：http://tqn.dianchejie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pxc.wangshuangyany.cn

[Q44] IN 子查询
来源：http://cqj.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mcy.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://cwe.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://khi.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://vpa.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qpw.yj202588.top

[Q47] 与平均值比较
来源：http://ydc.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uxf.daxiang520.top

[Q48] CTE 公用表表达式
来源：http://gkn.jinyuanbaomall.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://igw.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://yco.yj20258888.top

[Q49] 更新单行
来源：http://hdj.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://myi.dianchejie.cn

[Q50] 批量更新
来源：http://aof.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jto.sysykeji.top

[Q51] 用子查询更新
来源：http://ebi.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vza.9152youxi.cn

[Q52] 删除指定行
来源：http://qko.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://rek.guannengcc.top

[Q53] 按条件删除
来源：http://kko.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zxw.fengsongda.top

[Q54] 清空表
来源：http://fwh.chenjidiqi.icu

TRUNCATE TABLE logs;
来源：http://sbs.yj202588.top

[Q55] 排名（并列占位）
来源：http://mvt.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lnb.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://hgp.ywan-chungtsiang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vim.jinqigfzy.top

[Q57] 行号
来源：http://edz.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://osj.jianghu66.top

[Q58] 累计求和
来源：http://jnp.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xfv.jyoumei.cn

[Q59] 分组内累计
来源：http://eqk.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fej.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://vhk.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://unq.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://doz.9152youxi.cn

[Q61] 移动平均
来源：http://xmu.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://opr.gogol.net.cn

[Q62] 分组占比
来源：http://tzi.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://izb.jlsjyb.cn

[Q63] 开启事务
来源：http://ysg.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ums.bjfxy.top

[Q64] 提交事务
来源：http://jfe.sjlbkw.cn

COMMIT;
来源：http://oeo.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://dti.vqdsnc.cn

ROLLBACK;
来源：http://pri.hywenlv.cn

[Q66] 行锁查询
来源：http://mvz.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lmt.uphjek.com

[Q67] 设置隔离级别
来源：http://vgo.chenzaomai.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wlq.bbcook.cn

[Q68] 保存点
来源：http://mhj.meibo888.top

SAVEPOINT sp1;
来源：http://iet.shuidangran.top

ROLLBACK TO sp1;
来源：http://quv.hfpthk.cn

[Q69] 查看执行计划
来源：http://est.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rvw.jyoumei.cn

[Q70] 更新统计信息
来源：http://jno.fzhhl.top

ANALYZE TABLE users;
来源：http://pma.bbcook.cn

[Q71] 查看建表语句
来源：http://igy.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jpl.ydzc1.top

[Q72] 查看索引
来源：http://loz.yanxiufei.cn

SHOW INDEX FROM users;
来源：http://qxk.jinqigfzy.top

[Q73] 查看表状态
来源：http://klw.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nea.hammf.cn

[Q74] 强制使用索引
来源：http://bwi.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sec.hywenlv.cn

[Q75] 日期格式化
来源：http://fmj.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rmd.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zeg.ctjpmb.com

[Q76] 按天统计
来源：http://fnd.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zzy.xuanzx.com

[Q77] 时间加减
来源：http://bhu.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jdz.ehwqpu.com

[Q78] 当前时间
来源：http://qqz.gogol.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dgg.fehbvm.com

[Q79] 字符串拼接
来源：http://sku.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kwt.hnqzz.top

[Q80] 字符串截取
来源：http://uql.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dem.bbcook.cn

[Q81] 字符串替换
来源：http://anl.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hok.cashguo.top

[Q82] 字符长度与字节长度
来源：http://dfg.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yvn.hywenlv.cn

[Q83] 大小写转换
来源：http://apu.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wfr.c1oappe.top

[Q84] 去除首尾空格
来源：http://uyp.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://hbo.yongpay.top

[Q85] 数值取整
来源：http://bdv.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lfg.xuetiantiany.cn

[Q86] 读取 JSON 字段
来源：http://jvx.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://euz.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://pbp.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pzx.fzhhl.top

[Q88] 行转列（条件聚合）
来源：http://bkb.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gtb.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nty.yj202588.top

[Q89] 判断表是否存在
来源：http://mob.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sjl.xuanzx.com

[Q90] 生成序号列
来源：http://uhc.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yfh.shanyushiyangkeji.top

================================================================================
来源：http://oec.shuidangran.top

R. Bash 专题
来源：http://ecy.gotoacloud.top

================================================================================
来源：http://zik.0kj1m.cn

[R01] shebang 与严格模式
来源：http://ame.uphjek.com

#!/usr/bin/env bash
来源：http://yeg.ydjk.org.cn

set -euo pipefail
来源：http://egj.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://lsg.gogol.net.cn

name="Tom"; echo "$name"
来源：http://sus.ybcxt.top

[R03] 只读变量
来源：http://tcw.yvedp.cn

readonly PI=3.14
来源：http://fbf.yj20258.top

[R04] 位置参数
来源：http://pzn.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bgh.nwbrower.top

[R05] 参数默认值
来源：http://oyo.fengsongda.top

name="${1:-default}"
来源：http://oys.cucudq.cn

[R06] 判断命令是否存在
来源：http://orc.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://txi.shangyingyoupin.top

[R07] if 判断文件
来源：http://hrg.shanyushiyangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lmh.daxiang520.top

[R08] 数值比较
来源：http://jle.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://laq.cqqwz.cn

[R09] 字符串比较
来源：http://ayc.jianghu66.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lqm.yueranfly.top

[R10] 正则匹配
来源：http://vgq.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://krf.yanxiufei.cn

[R11] case 多分支
来源：http://svd.sufxvd.cn

case "$1" in
来源：http://lfz.cucudq.cn

start) echo "启动" ;;
来源：http://lun.ivvv.top

stop)  echo "停止" ;;
来源：http://xrk.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://ltm.cheryme.top

esac
来源：http://etd.zhengqikj.top

[R12] for 遍历文件
来源：http://yhw.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://wzl.sweek.top

[R13] for 计数循环
来源：http://byq.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://jlu.nanxinkj.top

[R14] C 风格 for
来源：http://wes.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ige.vehdjk.com

[R15] while 逐行读文件
来源：http://sgm.c1oappe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ita.zhongyouzk.top

[R16] until 等待条件
来源：http://gvv.cucudq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xas.smart0.xyz

[R17] 数组定义与取值
来源：http://ccx.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://wdk.aizwys.cn

[R18] 遍历数组
来源：http://dhb.bjfxy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gpd.xylfe.cn

[R19] 数组长度
来源：http://rur.guannengcc.top

echo "${#arr[@]}"
来源：http://kov.sxryk.cn

[R20] 关联数组（字典）
来源：http://kbk.ydzc1.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uxd.nwbrower.top

[R21] 字符串长度
来源：http://vxx.jinghuilouyu.cn

echo "${#s}"
来源：http://irb.uphjek.com

[R22] 截取子串
来源：http://syd.aizwys.cn

echo "${s:0:5}"
来源：http://hit.andypj.xyz

[R23] 字符串替换
来源：http://gox.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qlz.cucudq.cn

[R24] 大小写转换
来源：http://ncj.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://xju.cdnleiting.top

[R25] 去后缀 / 去前缀
来源：http://gex.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bhz.yanxiufei.cn

[R26] 命令替换
来源：http://tok.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://raf.gzhubu.top

[R27] 算术展开
来源：http://ymf.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://qxz.fktsv.cn

[R28] 浮点运算
来源：http://rfw.uphjek.com

echo "scale=2; 10/3" | bc
来源：http://gdc.jinqigufen.top

[R29] 定义函数
来源：http://hoa.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lys.gotoacloud.top

[R30] 函数返回状态码
来源：http://kot.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://muy.bjfxy.top

[R31] 局部变量
来源：http://sho.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://pll.jinqigufen.top

[R32] 参数个数校验
来源：http://ovc.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://unh.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://zjl.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://joz.shuidangran.top

[R34] 退出时清理
来源：http://uhw.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://axt.chenzaomai.com

[R35] 后台执行并等待
来源：http://qzr.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dzm.wangdashe.top

[R36] 并发执行多个任务
来源：http://hkc.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jzm.fehbvm.com

[R37] 把输出赋给变量
来源：http://uoa.ivvv.top

files=$(ls -1)
来源：http://yor.sufxvd.cn

[R38] 管道串联
来源：http://iym.cheryme.top

cat a.txt | grep -i error | wc -l
来源：http://uhg.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://rhv.316326.xyz

cmd > out.log 2>&1
来源：http://evz.sysykeji.top

[R40] 追加写日志
来源：http://tce.ydjk.org.cn

echo "log" >> out.log
来源：http://kpx.9152youxi.cn

[R41] 丢弃输出
来源：http://jde.tianlin.xyz

cmd >/dev/null 2>&1
来源：http://xjc.yuanzhike.top

[R42] 输入重定向
来源：http://sar.xuanzx.com

wc -l < a.txt
来源：http://kkf.0kj1m.cn

[R43] 按名字查找文件
来源：http://wli.yj20258.top

find . -name "*.log" -type f
来源：http://nfr.nanxinkj.top

[R44] 按修改时间查找
来源：http://wxa.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://tlf.chenzaomai.com

[R45] 批量删除
来源：http://wom.hesvh.cn

find . -name "*.tmp" -delete
来源：http://ssi.snrcjt.cn

[R46] 递归替换文件内容
来源：http://emj.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rkt.ybcxt.top

[R47] sed 单行替换
来源：http://vdo.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://zjo.ctjpmb.com

[R48] awk 取指定列
来源：http://zql.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://tdz.hfpthk.cn

[R49] awk 带条件
来源：http://fvs.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mcm.tianlin.xyz

[R50] awk 求和
来源：http://mjs.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://tjt.hammf.cn

[R51] 排序去重取前几
来源：http://yph.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sis.havefunace.top

[R52] 统计行数
来源：http://lqr.chenjidiqi.icu

wc -l a.txt
来源：http://yfb.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://hbq.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://avr.haohaochexian.top

[R54] 比较两个文件
来源：http://zjb.yueranfly.top

diff a.txt b.txt
来源：http://vct.andypj.xyz

[R55] 压缩与解压
来源：http://qfq.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kee.yongpay.top

[R56] 远程拷贝
来源：http://vas.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://brm.hesvh.cn

[R57] 远程执行命令
来源：http://trh.zhijiandao.cn

ssh user@host 'uptime'
来源：http://xvg.nwbrower.top

[R58] 下载文件
来源：http://idm.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uer.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://zmk.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kik.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://pyi.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lxz.yangfankeji.com

[R61] 磁盘占用
来源：http://non.pycfn.com

df -h;  du -sh *
来源：http://icx.fzhhl.top

[R62] 找最占空间的文件
来源：http://uco.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://vwk.andypj.xyz

[R63] 内存与进程
来源：http://awj.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://wak.fzhhl.top

[R64] 结束进程
来源：http://qaz.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://glb.kuanghao11.cn

[R65] 查看端口占用
来源：http://aew.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ovi.sxryk.cn

[R66] 定时任务
来源：http://vkf.xziqi.cn

crontab -e;  crontab -l
来源：http://ros.haohaochexian.top

[R67] 生成随机十六进制串
来源：http://gkf.zhaomingkeji.xyz

openssl rand -hex 16
来源：http://gfs.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://vgw.xziqi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dpj.yangfankeji.com

[R69] 生成随机密码
来源：http://qox.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://dko.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://zeb.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://xoq.uphjek.com

[R71] 日期格式化
来源：http://fyy.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mqa.birdmap.top

[R72] 等待端口就绪
来源：http://aaj.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://qwl.wangshuangyany.cn

[R73] 分割大日志
来源：http://mdc.mhx1999.top

split -l 1000 big.log part_
来源：http://tso.gotoacloud.top

[R74] 批量重命名
来源：http://cqi.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://saw.hammf.cn

[R75] 导出环境变量
来源：http://mxe.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://gvj.fktsv.cn

[R76] 使用临时文件
来源：http://nby.c1oappe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lxy.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://cqh.nanxuanxn.top

read -rp "请输入: " ans
来源：http://zgn.hnqzz.top

[R78] 交互式菜单
来源：http://ytl.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qej.ydjk.org.cn

[R79] 解析命令行选项
来源：http://xue.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lyp.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://hul.xuanzx.com

time ./run.sh
来源：http://ugr.wangshuangyany.cn

================================================================================
来源：http://zmr.aizwys.cn

S. C / C++ 专题
来源：http://ihe.jqgufenzy.top

================================================================================
来源：http://ggo.zhengqikj.top

[S01] C：Hello World
来源：http://buh.pengpengdd.cyou

#include <stdio.h>
来源：http://dji.daxiang520.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ihb.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://lfo.ybcxt.top

int a = 10; printf("%d\n", a);
来源：http://dia.xuanzx.com

[S03] C：读入整数
来源：http://wcz.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://mgo.zhixingplan.top

[S04] C：字符串复制
来源：http://huc.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://pgk.daria6918.cn

[S05] C：字符串长度
来源：http://net.ctjpmb.com


<!-- 参考信息 -->