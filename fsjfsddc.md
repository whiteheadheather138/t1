代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://snv.zhijiandao.cn

) t WHERE rn = 1;
来源：http://ear.fengsongda.top

[Q35] 内连接
来源：http://mhb.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zbw.gzhubu.top

[Q36] 左连接
来源：http://zcs.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://myh.yangfankeji.com

[Q37] 右连接
来源：http://mfc.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://trg.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://gsh.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wkm.ivvv.top

[Q39] 自连接（查上下级）
来源：http://ory.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xvc.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jgg.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pit.yongpay.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jkf.fzhhl.top

[Q41] 多表连接
来源：http://pdv.52xcode.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ysn.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://bdt.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://sbt.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://kcb.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://bsh.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://efa.quarkkingdee.top

[Q43] 标量子查询
来源：http://prl.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wts.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://cxd.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qky.snrcjt.cn

[Q45] EXISTS 判断存在
来源：http://ohu.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dij.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wis.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://znx.gzhubu.top

[Q47] 与平均值比较
来源：http://geb.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xvd.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://rhi.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gck.zhijiandao.cn

SELECT * FROM t WHERE c > 5;
来源：http://ohx.xziqi.cn

[Q49] 更新单行
来源：http://nif.gaohongyu789.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rke.cqqwz.cn

[Q50] 批量更新
来源：http://adt.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tzn.jlsjyb.cn

[Q51] 用子查询更新
来源：http://eep.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://doy.zhoulong.xyz

[Q52] 删除指定行
来源：http://nbd.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://jyn.hfpthk.cn

[Q53] 按条件删除
来源：http://wxe.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kcj.dianchejie.cn

[Q54] 清空表
来源：http://yta.ydzc1.top

TRUNCATE TABLE logs;
来源：http://hqh.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://fof.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zjk.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://qew.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jrj.sysykeji.top

[Q57] 行号
来源：http://snq.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kes.feifeiyinyue.top

[Q58] 累计求和
来源：http://ckm.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nwm.shangyingyoupin.top

[Q59] 分组内累计
来源：http://vqm.cucudq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ihk.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://dls.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wag.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mit.316326.xyz

[Q61] 移动平均
来源：http://zzg.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fdy.dianchejie.cn

[Q62] 分组占比
来源：http://ono.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://obl.gotoacloud.top

[Q63] 开启事务
来源：http://ufk.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://clu.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://mip.fengsongda.top

COMMIT;
来源：http://bgi.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://dqt.yueranfly.top

ROLLBACK;
来源：http://pqr.tian-w.cn

[Q66] 行锁查询
来源：http://ike.fehbvm.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nul.guannengcc.top

[Q67] 设置隔离级别
来源：http://rhz.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ilv.daria6918.cn

[Q68] 保存点
来源：http://hzj.kuanghao11.cn

SAVEPOINT sp1;
来源：http://zjb.zhongyouzk.top

ROLLBACK TO sp1;
来源：http://yuk.fehbvm.com

[Q69] 查看执行计划
来源：http://omt.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zel.52xcode.cn

[Q70] 更新统计信息
来源：http://wbt.yfazqb.com

ANALYZE TABLE users;
来源：http://ezf.yonumen.top

[Q71] 查看建表语句
来源：http://lfm.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lae.jqgufenzy.top

[Q72] 查看索引
来源：http://epf.hongshengwenyu.top

SHOW INDEX FROM users;
来源：http://kmh.haohaochexian.top

[Q73] 查看表状态
来源：http://puc.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uyh.gotoacloud.top

[Q74] 强制使用索引
来源：http://jnb.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ykk.wangshuangyany.cn

[Q75] 日期格式化
来源：http://uzq.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ppy.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vux.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://egb.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vfp.sufxvd.cn

[Q77] 时间加减
来源：http://saf.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tmc.smart0.xyz

[Q78] 当前时间
来源：http://esp.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nfm.fehbvm.com

[Q79] 字符串拼接
来源：http://hcd.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vlj.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://gxf.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lio.zhaomingkeji.xyz

[Q81] 字符串替换
来源：http://ewh.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gwt.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://zqy.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nnr.svipenyu.cn

[Q83] 大小写转换
来源：http://jxm.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://raq.jiagoushi.top

[Q84] 去除首尾空格
来源：http://mez.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://fcc.cqqwz.cn

[Q85] 数值取整
来源：http://fld.zdqjudy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wvk.hongshengwenyu.top

[Q86] 读取 JSON 字段
来源：http://vbr.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tne.gzhubu.top

[Q87] JSON 字段做条件
来源：http://rqy.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bio.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://oqj.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lgz.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fdf.havefunace.top

[Q89] 判断表是否存在
来源：http://ejn.yfazqb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cgk.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://tbl.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jvc.9152youxi.cn

================================================================================
来源：http://pog.dashuyun.cn

R. Bash 专题
来源：http://hnb.daxiang520.top

================================================================================
来源：http://nxw.jqgfzy.top

[R01] shebang 与严格模式
来源：http://brl.aizwys.cn

#!/usr/bin/env bash
来源：http://jos.jinghuilouyu.cn

set -euo pipefail
来源：http://hzl.tarul.cn

[R02] 变量赋值与使用
来源：http://yka.ehwqpu.com

name="Tom"; echo "$name"
来源：http://zyf.shzxlz.cn

[R03] 只读变量
来源：http://ppl.zhongyouzk.top

readonly PI=3.14
来源：http://aeu.nanxinkj.top

[R04] 位置参数
来源：http://wrt.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oxy.fktsv.cn

[R05] 参数默认值
来源：http://jko.yonumen.top

name="${1:-default}"
来源：http://njy.shanyushiyangkeji.top

[R06] 判断命令是否存在
来源：http://afj.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rzk.ybcxt.top

[R07] if 判断文件
来源：http://vmi.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jle.chenlongwang.top

[R08] 数值比较
来源：http://htz.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://phe.vqdsnc.cn

[R09] 字符串比较
来源：http://wzl.tanke756.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cga.cucudq.cn

[R10] 正则匹配
来源：http://qhk.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vvi.zhongyouzk.top

[R11] case 多分支
来源：http://vuu.ehwqpu.com

case "$1" in
来源：http://vxz.sxryk.cn

start) echo "启动" ;;
来源：http://txe.sxryk.cn

stop)  echo "停止" ;;
来源：http://afs.jianghu66.top

*)     echo "未知命令" ;;
来源：http://vyj.zhijiandao.cn

esac
来源：http://ffn.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://qbn.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://ang.feifeiyinyue.top

[R13] for 计数循环
来源：http://cyx.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://eht.guowangkeji.top

[R14] C 风格 for
来源：http://pgn.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kxl.smart0.xyz

[R15] while 逐行读文件
来源：http://wde.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hta.yuxming.cn

[R16] until 等待条件
来源：http://qoa.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://txz.yueranfly.top

[R17] 数组定义与取值
来源：http://jqs.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hvk.ybcxt.top

[R18] 遍历数组
来源：http://zwp.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hum.aizwys.cn

[R19] 数组长度
来源：http://aju.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://zwo.andypj.xyz

[R20] 关联数组（字典）
来源：http://nfm.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://woj.epnwcf.com

[R21] 字符串长度
来源：http://cma.jinqigufen.top

echo "${#s}"
来源：http://prx.cucudq.cn

[R22] 截取子串
来源：http://bav.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://kqz.wangshuangyany.cn

[R23] 字符串替换
来源：http://jjt.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wcx.redwolf501.top

[R24] 大小写转换
来源：http://rvd.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ssv.jlsjyb.cn

[R25] 去后缀 / 去前缀
来源：http://weo.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://sah.yueranfly.top

[R26] 命令替换
来源：http://iqv.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://imo.hongshengwenyu.top

[R27] 算术展开
来源：http://loj.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://ypn.quarkkingdee.top

[R28] 浮点运算
来源：http://syo.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://pyt.0kj1m.cn

[R29] 定义函数
来源：http://myq.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pjb.jiagoushi.top

[R30] 函数返回状态码
来源：http://bcy.iojbl.cn

f() { return 0; }; f || echo "失败了"
来源：http://ocg.hnxiangtu.top

[R31] 局部变量
来源：http://uio.ydzc1.top

f() { local x=1; echo "$x"; }
来源：http://fbs.bjfxy.top

[R32] 参数个数校验
来源：http://qmc.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bek.meibo888.top

[R33] 捕获错误并提示行号
来源：http://dzj.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rel.hywenlv.cn

[R34] 退出时清理
来源：http://hve.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://aoe.yj202588.top

[R35] 后台执行并等待
来源：http://vrq.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ubl.fehbvm.com

[R36] 并发执行多个任务
来源：http://cqh.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://arj.sweek.top

[R37] 把输出赋给变量
来源：http://otb.guowangkeji.top

files=$(ls -1)
来源：http://vsx.ybcxt.top

[R38] 管道串联
来源：http://fpp.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://mqn.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://zia.jqgufenzy.top

cmd > out.log 2>&1
来源：http://fnu.jinghuilouyu.cn

[R40] 追加写日志
来源：http://toy.hywenlv.cn

echo "log" >> out.log
来源：http://hjh.feifeiyinyue.top

[R41] 丢弃输出
来源：http://nzn.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://nak.pengpengdd.cyou

[R42] 输入重定向
来源：http://fpu.zycfv.cn

wc -l < a.txt
来源：http://qwc.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://xvb.yj20258.top

find . -name "*.log" -type f
来源：http://pnq.tanke756.top

[R44] 按修改时间查找
来源：http://hgz.jinqigufen.top

find . -mtime -7 -type f
来源：http://fod.ppjwa.cn

[R45] 批量删除
来源：http://ryk.meibo888.top

find . -name "*.tmp" -delete
来源：http://tfj.zdbjq.cn

[R46] 递归替换文件内容
来源：http://lyd.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fmt.yueranfly.top

[R47] sed 单行替换
来源：http://buf.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://ypj.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://tdk.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://ocy.hfpthk.cn

[R49] awk 带条件
来源：http://yna.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bjh.gogol.net.cn

[R50] awk 求和
来源：http://pzu.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://nrt.haohaochexian.top

[R51] 排序去重取前几
来源：http://bbs.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ijo.chenjidiqi.icu

[R52] 统计行数
来源：http://ssi.ydjk.org.cn

wc -l a.txt
来源：http://ucf.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://rvz.gotoacloud.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ngt.jqgufenzy.top

[R54] 比较两个文件
来源：http://szd.guannengcc.top

diff a.txt b.txt
来源：http://oep.yangfankeji.com

[R55] 压缩与解压
来源：http://vnt.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://esn.jinqigfzy.top

[R56] 远程拷贝
来源：http://tss.yonumen.top

scp file user@host:/path/
来源：http://bls.nanxinkj.top

[R57] 远程执行命令
来源：http://ddk.9152youxi.cn

ssh user@host 'uptime'
来源：http://vol.uphjek.com

[R58] 下载文件
来源：http://exp.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ldo.yangfankeji.com

[R59] 发 POST JSON
来源：http://avq.bjfxy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tyh.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://bhn.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kto.yuxming.cn

[R61] 磁盘占用
来源：http://rcw.xuanzx.com

df -h;  du -sh *
来源：http://nhl.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://bbe.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://rft.shanyushiyangtech.top

[R63] 内存与进程
来源：http://khb.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://wbi.yvedp.cn

[R64] 结束进程
来源：http://qlg.gzhubu.top

kill -9 $(pgrep -f app.py)
来源：http://dnx.fktsv.cn

[R65] 查看端口占用
来源：http://unb.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iia.andypj.xyz

[R66] 定时任务
来源：http://vlt.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://kiz.fengsongda.top

[R67] 生成随机十六进制串
来源：http://pnf.ctjpmb.com

openssl rand -hex 16
来源：http://ezt.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://ddg.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://uui.zhijiandao.cn

[R69] 生成随机密码
来源：http://hgz.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://fca.zhijiandao.cn

[R70] 时间戳与互转
来源：http://ovi.pycfn.com

date +%s;  date -d @1700000000
来源：http://odp.c1oappe.top

[R71] 日期格式化
来源：http://oig.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://umy.jqgfzy.top

[R72] 等待端口就绪
来源：http://uxy.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://phs.yanxiufei.cn

[R73] 分割大日志
来源：http://rnp.jqgufenzy.top

split -l 1000 big.log part_
来源：http://rwl.gotoacloud.top

[R74] 批量重命名
来源：http://ndt.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://slk.zhixingplan.top

[R75] 导出环境变量
来源：http://jvw.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://qpk.316326.xyz

[R76] 使用临时文件
来源：http://bgq.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://utw.havefunace.top

[R77] 读取用户输入
来源：http://our.tanke756.top

read -rp "请输入: " ans
来源：http://ioz.yvedp.cn

[R78] 交互式菜单
来源：http://zuz.316326.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://ujk.yj20258888.top

[R79] 解析命令行选项
来源：http://kwu.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lkd.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://vww.fehbvm.com

time ./run.sh
来源：http://ccx.epnwcf.com

================================================================================
来源：http://kot.jinqigfzy.top

S. C / C++ 专题
来源：http://qtl.zhiwuduotai.top

================================================================================
来源：http://aef.guannengcc.top

[S01] C：Hello World
来源：http://hfg.meibo888.top

#include <stdio.h>
来源：http://qls.shuidangran.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nlm.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://qtx.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://yvv.cashguo.top

[S03] C：读入整数
来源：http://jft.wangshuangyany.cn


<!-- 参考信息 -->