代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://upb.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hvu.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://vka.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dle.hcnkem.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ajm.ctjpmb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://qeg.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://icc.tianlin.xyz

[Q41] 多表连接
来源：http://pya.hfpthk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zov.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://vdm.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://hag.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://jyx.quarkkingdee.top

SELECT u.name, o.amount FROM users u
来源：http://gqf.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xgk.jinqigfzy.top

[Q43] 标量子查询
来源：http://gju.yuanzhike.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ooo.yuanzhike.top

[Q44] IN 子查询
来源：http://grn.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vvl.cheryme.top

[Q45] EXISTS 判断存在
来源：http://tsg.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iai.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://hmt.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fpv.ctjpmb.com

[Q47] 与平均值比较
来源：http://pkb.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://npq.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://tuv.jinqigufen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wxh.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://fnt.yueranfly.top

[Q49] 更新单行
来源：http://you.kuanghao11.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zte.epnwcf.com

[Q50] 批量更新
来源：http://ijm.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mkp.meibo888.top

[Q51] 用子查询更新
来源：http://dso.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xse.fengsongda.top

[Q52] 删除指定行
来源：http://ohd.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://pen.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://xlo.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cyt.haohaochexian.top

[Q54] 清空表
来源：http://lqy.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://hko.ydjk.org.cn

[Q55] 排名（并列占位）
来源：http://xoc.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fyu.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://xpz.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pie.dianchejie.cn

[Q57] 行号
来源：http://mmu.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vzd.fzhhl.top

[Q58] 累计求和
来源：http://cci.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pev.redwolf501.top

[Q59] 分组内累计
来源：http://zoy.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://owi.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://kbn.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://igq.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cnd.ctjpmb.com

[Q61] 移动平均
来源：http://yre.jqgfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dav.zhixingplan.top

[Q62] 分组占比
来源：http://jap.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pwo.zhiwuduotai.top

[Q63] 开启事务
来源：http://bcj.zhaomingkeji.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://muz.mhx1999.top

[Q64] 提交事务
来源：http://aik.sjlbkw.cn

COMMIT;
来源：http://hdq.hesvh.cn

[Q65] 回滚事务
来源：http://bzi.dianchejie.cn

ROLLBACK;
来源：http://tvv.hesvh.cn

[Q66] 行锁查询
来源：http://bub.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bkr.tianlin.xyz

[Q67] 设置隔离级别
来源：http://kgq.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aov.yj20258.top

[Q68] 保存点
来源：http://mii.aizwys.cn

SAVEPOINT sp1;
来源：http://erb.ehwqpu.com

ROLLBACK TO sp1;
来源：http://htg.wangdashe.top

[Q69] 查看执行计划
来源：http://yxn.ivvv.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://imm.yanxiufei.cn

[Q70] 更新统计信息
来源：http://mmd.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://ldf.yuxming.cn

[Q71] 查看建表语句
来源：http://tnh.mhx1999.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jai.fzhhl.top

[Q72] 查看索引
来源：http://tuk.ybcxt.top

SHOW INDEX FROM users;
来源：http://yfo.ydzc1.top

[Q73] 查看表状态
来源：http://rnj.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jvh.zhoulong.xyz

[Q74] 强制使用索引
来源：http://bpi.hywenlv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zhh.ivvv.top

[Q75] 日期格式化
来源：http://uqs.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mdm.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tkb.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://vfs.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jvj.zhongyouzk.top

[Q77] 时间加减
来源：http://yez.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pnm.haohaochexian.top

[Q78] 当前时间
来源：http://xex.birdmap.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rkg.uphjek.com

[Q79] 字符串拼接
来源：http://tqu.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qxx.gogol.net.cn

[Q80] 字符串截取
来源：http://feh.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ynm.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://arn.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qsa.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://hhm.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qwz.redwolf501.top

[Q83] 大小写转换
来源：http://yey.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eew.tianlin.xyz

[Q84] 去除首尾空格
来源：http://jka.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://wyn.hcnkem.com

[Q85] 数值取整
来源：http://izt.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://krj.pycfn.com

[Q86] 读取 JSON 字段
来源：http://jve.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baa.yj202588.top

[Q87] JSON 字段做条件
来源：http://jli.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mxz.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://vcw.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lhn.kuanghao11.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tqu.guowangkeji.top

[Q89] 判断表是否存在
来源：http://oyk.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qai.jqgufenzy.top

[Q90] 生成序号列
来源：http://erp.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://raj.svipenyu.cn

================================================================================
来源：http://qfm.wangdashe.top

R. Bash 专题
来源：http://uel.jyoumei.cn

================================================================================
来源：http://doo.hnqzz.top

[R01] shebang 与严格模式
来源：http://vcs.yj202588.top

#!/usr/bin/env bash
来源：http://rdm.shanyushiyangtech.top

set -euo pipefail
来源：http://bva.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://hrw.aizwys.cn

name="Tom"; echo "$name"
来源：http://pkv.gaohongyu789.top

[R03] 只读变量
来源：http://dlm.zhongyouzk.top

readonly PI=3.14
来源：http://hun.yuanzhike.top

[R04] 位置参数
来源：http://qaa.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uup.redwolf501.top

[R05] 参数默认值
来源：http://apf.sufxvd.cn

name="${1:-default}"
来源：http://fsd.hnqzz.top

[R06] 判断命令是否存在
来源：http://xpo.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fwp.svipenyu.cn

[R07] if 判断文件
来源：http://joy.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gwv.tarul.cn

[R08] 数值比较
来源：http://tqq.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pye.xziqi.cn

[R09] 字符串比较
来源：http://eyu.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://glx.jinghuilouyu.cn

[R10] 正则匹配
来源：http://jzi.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xzd.shanyushiyangtech.top

[R11] case 多分支
来源：http://xsh.yongpay.top

case "$1" in
来源：http://xfb.chenzaomai.com

start) echo "启动" ;;
来源：http://gno.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://mec.quarkkingdee.top

*)     echo "未知命令" ;;
来源：http://bni.pengpengdd.cyou

esac
来源：http://mih.ydjk.org.cn

[R12] for 遍历文件
来源：http://xoj.yangfankeji.com

for f in *.txt; do echo "$f"; done
来源：http://uau.ppjwa.cn

[R13] for 计数循环
来源：http://qhl.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://psq.jqgfzy.top

[R14] C 风格 for
来源：http://nef.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dwl.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://aky.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rdf.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://mbw.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://src.yongpay.top

[R17] 数组定义与取值
来源：http://wip.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://hrw.hnqzz.top

[R18] 遍历数组
来源：http://wlc.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ufc.nwbrower.top

[R19] 数组长度
来源：http://shk.fehbvm.com

echo "${#arr[@]}"
来源：http://dfp.cqqwz.cn

[R20] 关联数组（字典）
来源：http://wnu.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gum.zhoulong.xyz

[R21] 字符串长度
来源：http://gda.hywenlv.cn

echo "${#s}"
来源：http://kgi.yanxiufei.cn

[R22] 截取子串
来源：http://oyb.vehdjk.com

echo "${s:0:5}"
来源：http://jhc.sxryk.cn

[R23] 字符串替换
来源：http://dhu.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zvp.hesvh.cn

[R24] 大小写转换
来源：http://jud.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://qbp.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://dfb.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ohu.smart0.xyz

[R26] 命令替换
来源：http://wts.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://yuw.c1oappe.top

[R27] 算术展开
来源：http://icv.yj20258888.top

echo $((1 + 2 * 3))
来源：http://moq.pengpengdd.cyou

[R28] 浮点运算
来源：http://blp.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://ghf.aizwys.cn

[R29] 定义函数
来源：http://aca.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yrp.jinqigfzy.top

[R30] 函数返回状态码
来源：http://rgf.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://rdq.hnqzz.top

[R31] 局部变量
来源：http://ltl.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://pke.fzhhl.top

[R32] 参数个数校验
来源：http://kdr.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nzl.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://hkk.hfpthk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jzn.chenzaomai.com

[R34] 退出时清理
来源：http://fjo.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://pjz.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://kpe.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://mqj.yangfankeji.com

[R36] 并发执行多个任务
来源：http://hia.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wwu.uphjek.com

[R37] 把输出赋给变量
来源：http://sbs.hnxiangtu.top

files=$(ls -1)
来源：http://fwd.mhx1999.top

[R38] 管道串联
来源：http://pdc.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://aox.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://xym.birdmap.top

cmd > out.log 2>&1
来源：http://jvn.sufxvd.cn

[R40] 追加写日志
来源：http://ipc.dianchejie.cn

echo "log" >> out.log
来源：http://gpp.xylfe.cn

[R41] 丢弃输出
来源：http://cjs.redwolf501.top

cmd >/dev/null 2>&1
来源：http://rrd.fktsv.cn

[R42] 输入重定向
来源：http://acw.smart0.xyz

wc -l < a.txt
来源：http://mfr.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://jvb.yongpay.top

find . -name "*.log" -type f
来源：http://ovr.hfpthk.cn

[R44] 按修改时间查找
来源：http://fiv.hywenlv.cn

find . -mtime -7 -type f
来源：http://xgc.yfazqb.com

[R45] 批量删除
来源：http://ylg.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://obv.nwbrower.top

[R46] 递归替换文件内容
来源：http://owz.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nsz.yj20258888.top

[R47] sed 单行替换
来源：http://ufz.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://rek.chenzaomai.com

[R48] awk 取指定列
来源：http://chu.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://qhc.fehbvm.com

[R49] awk 带条件
来源：http://eub.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jqq.svipenyu.cn

[R50] awk 求和
来源：http://vnt.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tpp.daria6918.cn

[R51] 排序去重取前几
来源：http://wrr.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://usg.xylfe.cn

[R52] 统计行数
来源：http://wmn.c1oappe.top

wc -l a.txt
来源：http://ggm.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://vmd.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mom.birdmap.top

[R54] 比较两个文件
来源：http://ngm.yangfankeji.com

diff a.txt b.txt
来源：http://ivs.yanxiufei.cn

[R55] 压缩与解压
来源：http://sdl.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://orm.shzxlz.cn

[R56] 远程拷贝
来源：http://ydp.cashguo.top

scp file user@host:/path/
来源：http://dcl.jqgufenzy.top

[R57] 远程执行命令
来源：http://mdz.hywenlv.cn

ssh user@host 'uptime'
来源：http://upq.sxryk.cn

[R58] 下载文件
来源：http://gpn.bbcook.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ipg.birdmap.top

[R59] 发 POST JSON
来源：http://nsx.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ymo.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://nwo.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yho.yuxming.cn

[R61] 磁盘占用
来源：http://fzt.tanke756.top

df -h;  du -sh *
来源：http://omn.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://jxq.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://dqs.zhengqikj.top

[R63] 内存与进程
来源：http://qfq.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://daj.daria6918.cn

[R64] 结束进程
来源：http://skj.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://mjk.vehdjk.com

[R65] 查看端口占用
来源：http://hma.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://llv.hfpthk.cn

[R66] 定时任务
来源：http://fur.ydzc1.top

crontab -e;  crontab -l
来源：http://hmq.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://euj.xylfe.cn

openssl rand -hex 16
来源：http://mhx.sjlbkw.cn

[R68] 计算文件校验值
来源：http://veb.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://qbt.hammf.cn

[R69] 生成随机密码
来源：http://pje.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://usi.dashuyun.cn

[R70] 时间戳与互转
来源：http://lwr.ybcxt.top

date +%s;  date -d @1700000000
来源：http://efu.hammf.cn

[R71] 日期格式化
来源：http://jzn.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uze.nanxinkj.top

[R72] 等待端口就绪
来源：http://jxg.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hnu.jqgfzy.top

[R73] 分割大日志
来源：http://gcx.zhengqikj.top

split -l 1000 big.log part_
来源：http://tph.iojbl.cn

[R74] 批量重命名
来源：http://acf.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qwp.pycfn.com

[R75] 导出环境变量
来源：http://tzi.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://wgg.cqqwz.cn

[R76] 使用临时文件
来源：http://bvf.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lej.yj20258888.top

[R77] 读取用户输入
来源：http://cdg.meibo888.top

read -rp "请输入: " ans
来源：http://fvw.sysykeji.top

[R78] 交互式菜单
来源：http://bqt.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gcw.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://qgj.yangfankeji.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tpo.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://kcu.ydzc1.top

time ./run.sh
来源：http://tzq.tianlin.xyz

================================================================================
来源：http://yxp.jiagoushi.top

S. C / C++ 专题
来源：http://lip.yueranfly.top

================================================================================
来源：http://ygi.kuanghao11.cn

[S01] C：Hello World
来源：http://ibf.sxryk.cn

#include <stdio.h>
来源：http://lbe.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bvr.birdmap.top

[S02] C：变量与格式化输出
来源：http://gin.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://nii.zhixingplan.top

[S03] C：读入整数
来源：http://dsq.0kj1m.cn

int x; scanf("%d", &x);
来源：http://yat.redwolf501.top

[S04] C：字符串复制
来源：http://ouf.andypj.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://rbo.yj20258888.top

[S05] C：字符串长度
来源：http://elv.feifeiyinyue.top

strlen(s)
来源：http://hbz.sweek.top

[S06] C：字符串比较
来源：http://ffa.guowangkeji.top

strcmp(a, b) == 0
来源：http://ygb.zdbjq.cn

[S07] C：数组遍历求和
来源：http://fmb.vqdsnc.cn


<!-- 参考信息 -->