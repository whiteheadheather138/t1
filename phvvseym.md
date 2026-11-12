代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://ydq.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rlu.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://wse.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://luy.bjfxy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ajb.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iek.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://izl.gaohongyu789.top

[Q41] 多表连接
来源：http://lvr.quarkkingdee.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wmr.guannengcc.top

JOIN users u ON u.id = o.user_id
来源：http://mlw.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://bsr.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://hbu.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://vex.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jbc.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://wow.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uie.cqqwz.cn

[Q44] IN 子查询
来源：http://ozo.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wdf.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://dkw.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://txx.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://wgt.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jcu.hongshengwenyu.top

[Q47] 与平均值比较
来源：http://vmw.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iop.tanke756.top

[Q48] CTE 公用表表达式
来源：http://upi.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nfu.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://qza.jqgufenzy.top

[Q49] 更新单行
来源：http://szn.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hbt.zhoulong.xyz

[Q50] 批量更新
来源：http://kcb.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vpk.gogol.net.cn

[Q51] 用子查询更新
来源：http://tni.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jeb.redwolf501.top

[Q52] 删除指定行
来源：http://gdb.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://hhd.ctjpmb.com

[Q53] 按条件删除
来源：http://lzj.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zpv.iojbl.cn

[Q54] 清空表
来源：http://cxp.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://xef.fengsongda.top

[Q55] 排名（并列占位）
来源：http://vtt.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://noq.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://nzl.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wcn.ydjk.org.cn

[Q57] 行号
来源：http://idx.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wzh.nanxuanxn.top

[Q58] 累计求和
来源：http://rlg.0kj1m.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ioz.kuanghao11.cn

[Q59] 分组内累计
来源：http://hra.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ged.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://hfo.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pkt.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iwu.nwbrower.top

[Q61] 移动平均
来源：http://trh.wangshuangyany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://irw.pycfn.com

[Q62] 分组占比
来源：http://slf.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gvn.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://fzk.nanxinkj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tlc.hysaishi.cn

[Q64] 提交事务
来源：http://bjq.fengsongda.top

COMMIT;
来源：http://jqz.daria6918.cn

[Q65] 回滚事务
来源：http://fmq.fengsongda.top

ROLLBACK;
来源：http://yoo.aizwys.cn

[Q66] 行锁查询
来源：http://lqb.zhoulong.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://alr.zdbjq.cn

[Q67] 设置隔离级别
来源：http://zbw.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://szn.yfazqb.com

[Q68] 保存点
来源：http://jip.cucudq.cn

SAVEPOINT sp1;
来源：http://thr.yfazqb.com

ROLLBACK TO sp1;
来源：http://nxe.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://irv.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ehv.zdqjudy.top

[Q70] 更新统计信息
来源：http://ubx.hfpthk.cn

ANALYZE TABLE users;
来源：http://ulo.0kj1m.cn

[Q71] 查看建表语句
来源：http://yxk.guannengcc.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ljz.gogol.net.cn

[Q72] 查看索引
来源：http://kwn.yuxming.cn

SHOW INDEX FROM users;
来源：http://orl.316326.xyz

[Q73] 查看表状态
来源：http://wgo.epnwcf.com

SHOW TABLE STATUS LIKE 'users';
来源：http://qne.vehdjk.com

[Q74] 强制使用索引
来源：http://rnx.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cjn.wangshuangyany.cn

[Q75] 日期格式化
来源：http://pdv.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://doz.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://efb.hysaishi.cn

[Q76] 按天统计
来源：http://rnb.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vsr.zhongyouzk.top

[Q77] 时间加减
来源：http://hur.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oty.shzxlz.cn

[Q78] 当前时间
来源：http://xjx.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://idw.yanxiufei.cn

[Q79] 字符串拼接
来源：http://ouj.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bhc.cashguo.top

[Q80] 字符串截取
来源：http://dho.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://prb.zhoulong.xyz

[Q81] 字符串替换
来源：http://mbw.316326.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xqw.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://syf.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jzc.zhoulong.xyz

[Q83] 大小写转换
来源：http://wlj.uphjek.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gva.fktsv.cn

[Q84] 去除首尾空格
来源：http://shf.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://tuo.xziqi.cn

[Q85] 数值取整
来源：http://ppw.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hky.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://wjw.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dgm.hammf.cn

[Q87] JSON 字段做条件
来源：http://zpg.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rcl.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://dez.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jne.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gyr.gotoacloud.top

[Q89] 判断表是否存在
来源：http://lfi.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tpx.bjfxy.top

[Q90] 生成序号列
来源：http://gsn.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qry.ywan-chungtsiang.top

================================================================================
来源：http://uhq.epnwcf.com

R. Bash 专题
来源：http://xyd.xingfuxueyuan.xyz

================================================================================
来源：http://bju.ppjwa.cn

[R01] shebang 与严格模式
来源：http://ueo.vqdsnc.cn

#!/usr/bin/env bash
来源：http://aky.wangshuangyany.cn

set -euo pipefail
来源：http://vwj.cucudq.cn

[R02] 变量赋值与使用
来源：http://bki.cucudq.cn

name="Tom"; echo "$name"
来源：http://jsh.yanxiufei.cn

[R03] 只读变量
来源：http://iys.chenlongwang.top

readonly PI=3.14
来源：http://kim.fengsongda.top

[R04] 位置参数
来源：http://xcb.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yuj.gaohongyu789.top

[R05] 参数默认值
来源：http://mhp.zhongyouzk.top

name="${1:-default}"
来源：http://bah.guannengcc.top

[R06] 判断命令是否存在
来源：http://lku.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ell.dianchejie.cn

[R07] if 判断文件
来源：http://zkq.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blv.shanyushiyangkeji.top

[R08] 数值比较
来源：http://nxy.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dys.sjlbkw.cn

[R09] 字符串比较
来源：http://jfd.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nyw.ydzc1.top

[R10] 正则匹配
来源：http://bez.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pzl.tarul.cn

[R11] case 多分支
来源：http://qpj.smart0.xyz

case "$1" in
来源：http://tay.yj202588.top

start) echo "启动" ;;
来源：http://krc.guowangkeji.top

stop)  echo "停止" ;;
来源：http://kpa.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://ogk.jinqigufen.top

esac
来源：http://gii.hesvh.cn

[R12] for 遍历文件
来源：http://dzn.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://jja.jyoumei.cn

[R13] for 计数循环
来源：http://qza.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://wld.tian-w.cn

[R14] C 风格 for
来源：http://xtd.nanxuanxn.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lae.vqdsnc.cn

[R15] while 逐行读文件
来源：http://jic.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jir.chenjidiqi.icu

[R16] until 等待条件
来源：http://muu.havefunace.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iyz.vqdsnc.cn

[R17] 数组定义与取值
来源：http://zmf.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://vkk.chenjidiqi.icu

[R18] 遍历数组
来源：http://hkx.vqdsnc.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gui.zdbjq.cn

[R19] 数组长度
来源：http://edv.zhixingplan.top

echo "${#arr[@]}"
来源：http://ofb.hnqzz.top

[R20] 关联数组（字典）
来源：http://qga.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nhd.chenzaomai.com

[R21] 字符串长度
来源：http://bwu.chenzaomai.com

echo "${#s}"
来源：http://zok.ppjwa.cn

[R22] 截取子串
来源：http://xvz.0kj1m.cn

echo "${s:0:5}"
来源：http://qtd.hammf.cn

[R23] 字符串替换
来源：http://lcq.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uzi.jinqigufen.top

[R24] 大小写转换
来源：http://jqo.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://son.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://jqp.cdnleiting.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oqb.iojbl.cn

[R26] 命令替换
来源：http://odw.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://iih.epnwcf.com

[R27] 算术展开
来源：http://mwl.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://hnb.ydzc1.top

[R28] 浮点运算
来源：http://dhq.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://dpn.hysaishi.cn

[R29] 定义函数
来源：http://qpy.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cuk.yueranfly.top

[R30] 函数返回状态码
来源：http://udt.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://qqb.ywan-chungtsiang.top

[R31] 局部变量
来源：http://sre.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://zdp.zhoulong.xyz

[R32] 参数个数校验
来源：http://lpo.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kww.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://gjn.gogol.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dff.yj20258.top

[R34] 退出时清理
来源：http://zjc.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qkx.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://ful.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ipw.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://kcn.hywenlv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ahg.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://cly.ydzc1.top

files=$(ls -1)
来源：http://ieb.shangyingyoupin.top

[R38] 管道串联
来源：http://mjh.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://uuy.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://vgl.cashguo.top

cmd > out.log 2>&1
来源：http://ugk.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://izt.xuanzx.com

echo "log" >> out.log
来源：http://ibl.havefunace.top

[R41] 丢弃输出
来源：http://bpo.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://zfr.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://mbs.cdnleiting.top

wc -l < a.txt
来源：http://syr.hnxiangtu.top

[R43] 按名字查找文件
来源：http://pru.vqdsnc.cn

find . -name "*.log" -type f
来源：http://naj.zhongyouzk.top

[R44] 按修改时间查找
来源：http://stn.nanxinkj.top

find . -mtime -7 -type f
来源：http://ile.kuanghao11.cn

[R45] 批量删除
来源：http://toe.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://pxs.jianghu66.top

[R46] 递归替换文件内容
来源：http://hti.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fzd.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://qtn.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://dpz.uphjek.com

[R48] awk 取指定列
来源：http://gtm.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://myv.ppjwa.cn

[R49] awk 带条件
来源：http://zfc.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fxl.yj20258.top

[R50] awk 求和
来源：http://cmw.hfpthk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eiq.yvedp.cn

[R51] 排序去重取前几
来源：http://dkp.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://frv.sysykeji.top

[R52] 统计行数
来源：http://als.kuanghao11.cn

wc -l a.txt
来源：http://hqr.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://kcy.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bdg.hongshengwenyu.top

[R54] 比较两个文件
来源：http://rla.cashguo.top

diff a.txt b.txt
来源：http://duv.vehdjk.com

[R55] 压缩与解压
来源：http://euq.jinyuanbaomall.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zzc.bbcook.cn

[R56] 远程拷贝
来源：http://ezj.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://fsr.bbcook.cn

[R57] 远程执行命令
来源：http://ikt.yfazqb.com

ssh user@host 'uptime'
来源：http://gzn.andypj.xyz

[R58] 下载文件
来源：http://dnb.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jgq.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://rmu.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://feu.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://fbh.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ymg.hysaishi.cn

[R61] 磁盘占用
来源：http://atk.meibo888.top

df -h;  du -sh *
来源：http://wpa.iojbl.cn

[R62] 找最占空间的文件
来源：http://kzj.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://lbu.yongpay.top

[R63] 内存与进程
来源：http://sql.hesvh.cn

free -h;  ps aux | grep nginx
来源：http://bna.pycfn.com

[R64] 结束进程
来源：http://ewr.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://gkf.zhengqikj.top

[R65] 查看端口占用
来源：http://vbn.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wbu.jinqigfzy.top

[R66] 定时任务
来源：http://wbm.chenzaomai.com

crontab -e;  crontab -l
来源：http://vep.havefunace.top

[R67] 生成随机十六进制串
来源：http://rfr.zhijiandao.cn

openssl rand -hex 16
来源：http://fwu.jyoumei.cn

[R68] 计算文件校验值
来源：http://kqd.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rtk.redwolf501.top

[R69] 生成随机密码
来源：http://mzh.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://qkb.yj20258.top

[R70] 时间戳与互转
来源：http://rzy.fzhhl.top

date +%s;  date -d @1700000000
来源：http://qbn.shanyushiyangtech.top

[R71] 日期格式化
来源：http://bkz.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qdd.havefunace.top

[R72] 等待端口就绪
来源：http://rbi.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://erg.fengsongda.top

[R73] 分割大日志
来源：http://cfz.yfazqb.com

split -l 1000 big.log part_
来源：http://ake.hammf.cn

[R74] 批量重命名
来源：http://hcy.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://efv.9152youxi.cn

[R75] 导出环境变量
来源：http://upb.ydjk.org.cn

export PATH="$HOME/bin:$PATH"
来源：http://jqa.guowangkeji.top

[R76] 使用临时文件
来源：http://hrb.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://adl.yangfankeji.com

[R77] 读取用户输入
来源：http://wge.hesvh.cn

read -rp "请输入: " ans
来源：http://fti.pycfn.com

[R78] 交互式菜单
来源：http://njo.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://lzi.zhixingplan.top

[R79] 解析命令行选项
来源：http://ujw.0kj1m.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://djb.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://zih.cheryme.top

time ./run.sh
来源：http://san.pengpengdd.cyou

================================================================================
来源：http://ghx.hcnkem.com

S. C / C++ 专题
来源：http://cqt.9152youxi.cn

================================================================================
来源：http://okx.bjfxy.top

[S01] C：Hello World
来源：http://rex.yj20258.top

#include <stdio.h>
来源：http://gnp.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ley.uphjek.com

[S02] C：变量与格式化输出
来源：http://clk.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://mul.guowangkeji.top

[S03] C：读入整数
来源：http://gpj.tanke756.top

int x; scanf("%d", &x);
来源：http://qxq.yj202588.top

[S04] C：字符串复制
来源：http://uox.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jpw.tianlin.xyz

[S05] C：字符串长度
来源：http://sob.kuanghao11.cn

strlen(s)
来源：http://zwm.dashuyun.cn

[S06] C：字符串比较
来源：http://edd.yuxming.cn

strcmp(a, b) == 0
来源：http://rer.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://bbj.sweek.top


<!-- 参考信息 -->