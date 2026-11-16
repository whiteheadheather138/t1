代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://oyz.sjlbkw.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uso.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://ihv.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://res.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bom.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wjs.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ise.sweek.top

[Q41] 多表连接
来源：http://fzu.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ijp.dashuyun.cn

JOIN users u ON u.id = o.user_id
来源：http://vbw.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://hrf.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://jnz.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://wee.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ckc.sxryk.cn

[Q43] 标量子查询
来源：http://sec.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bij.haohaochexian.top

[Q44] IN 子查询
来源：http://egl.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ipr.dashuyun.cn

[Q45] EXISTS 判断存在
来源：http://rqm.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zvf.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://wjz.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xee.haohaochexian.top

[Q47] 与平均值比较
来源：http://iai.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lxb.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://tgc.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vmu.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://any.daxiang520.top

[Q49] 更新单行
来源：http://ybf.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xvs.52xcode.cn

[Q50] 批量更新
来源：http://pkn.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gae.yonumen.top

[Q51] 用子查询更新
来源：http://ozw.kuanghao11.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tlk.nwbrower.top

[Q52] 删除指定行
来源：http://ujp.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://ebc.shuidangran.top

[Q53] 按条件删除
来源：http://nqc.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qtj.yfazqb.com

[Q54] 清空表
来源：http://vpa.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://tku.cheryme.top

[Q55] 排名（并列占位）
来源：http://pkf.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://szd.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://ktn.yfazqb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eia.wangdashe.top

[Q57] 行号
来源：http://pqu.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tbi.tianlin.xyz

[Q58] 累计求和
来源：http://rsg.cucudq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fvo.iojbl.cn

[Q59] 分组内累计
来源：http://ljj.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ytl.hysaishi.cn

[Q60] 取上一行 / 下一行
来源：http://umq.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dxd.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xaf.wangshuangyany.cn

[Q61] 移动平均
来源：http://nas.tanke756.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fjz.xinyue.icu

[Q62] 分组占比
来源：http://htw.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mzk.nwbrower.top

[Q63] 开启事务
来源：http://mvo.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oab.dashuyun.cn

[Q64] 提交事务
来源：http://hob.ydjk.org.cn

COMMIT;
来源：http://sld.feifeiyinyue.top

[Q65] 回滚事务
来源：http://wxh.jinqigfzy.top

ROLLBACK;
来源：http://vgm.feifeiyinyue.top

[Q66] 行锁查询
来源：http://muj.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hsu.jiagoushi.top

[Q67] 设置隔离级别
来源：http://kec.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ecg.zhiwuduotai.top

[Q68] 保存点
来源：http://fkb.fehbvm.com

SAVEPOINT sp1;
来源：http://seq.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://kpg.snrcjt.cn

[Q69] 查看执行计划
来源：http://uwo.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://urw.smart0.xyz

[Q70] 更新统计信息
来源：http://mge.haohaochexian.top

ANALYZE TABLE users;
来源：http://xig.epnwcf.com

[Q71] 查看建表语句
来源：http://wjf.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://okh.zhiwuduotai.top

[Q72] 查看索引
来源：http://gmx.yj20258.top

SHOW INDEX FROM users;
来源：http://nzv.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://giw.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rqy.xylfe.cn

[Q74] 强制使用索引
来源：http://obd.xuetiantiany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gny.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://xgn.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zbo.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gtu.snrcjt.cn

[Q76] 按天统计
来源：http://wjb.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://stl.yuxming.cn

[Q77] 时间加减
来源：http://bbj.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gnx.zhoulong.xyz

[Q78] 当前时间
来源：http://vjc.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fui.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://jot.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jyf.gzhubu.top

[Q80] 字符串截取
来源：http://taz.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hyh.fehbvm.com

[Q81] 字符串替换
来源：http://dir.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fqo.uphjek.com

[Q82] 字符长度与字节长度
来源：http://fzm.wangdashe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ffy.hongshengwenyu.top

[Q83] 大小写转换
来源：http://xyb.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://viv.cqqwz.cn

[Q84] 去除首尾空格
来源：http://zot.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://ozw.hnxiangtu.top

[Q85] 数值取整
来源：http://cxw.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iuj.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://brb.sufxvd.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ejz.xylfe.cn

[Q87] JSON 字段做条件
来源：http://owd.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://suz.jinqigufen.top

[Q88] 行转列（条件聚合）
来源：http://lpa.jianghu66.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fid.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ibc.yueranfly.top

[Q89] 判断表是否存在
来源：http://byr.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tpc.bbcook.cn

[Q90] 生成序号列
来源：http://ral.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zsh.zhiwuduotai.top

================================================================================
来源：http://abe.ctjpmb.com

R. Bash 专题
来源：http://kge.ivvv.top

================================================================================
来源：http://jsf.chenjidiqi.icu

[R01] shebang 与严格模式
来源：http://ufx.uphjek.com

#!/usr/bin/env bash
来源：http://dtp.jinyuanbaomall.cn

set -euo pipefail
来源：http://fca.daxiang520.top

[R02] 变量赋值与使用
来源：http://wva.fktsv.cn

name="Tom"; echo "$name"
来源：http://spy.hesvh.cn

[R03] 只读变量
来源：http://akz.xuetiantiany.cn

readonly PI=3.14
来源：http://kjw.nanxinkj.top

[R04] 位置参数
来源：http://qdn.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://prs.hongshengwenyu.top

[R05] 参数默认值
来源：http://adv.guannengcc.top

name="${1:-default}"
来源：http://yfr.bjfxy.top

[R06] 判断命令是否存在
来源：http://gcj.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hns.vqdsnc.cn

[R07] if 判断文件
来源：http://xas.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://imf.cheryme.top

[R08] 数值比较
来源：http://ybl.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://scl.bbcook.cn

[R09] 字符串比较
来源：http://lji.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://emv.tianlin.xyz

[R10] 正则匹配
来源：http://nhc.yj20258.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qrl.ydjk.org.cn

[R11] case 多分支
来源：http://nrk.ybcxt.top

case "$1" in
来源：http://hng.ctjpmb.com

start) echo "启动" ;;
来源：http://sbz.c1oappe.top

stop)  echo "停止" ;;
来源：http://idq.epnwcf.com

*)     echo "未知命令" ;;
来源：http://nyk.ybcxt.top

esac
来源：http://atj.fktsv.cn

[R12] for 遍历文件
来源：http://ccx.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://jmj.hysaishi.cn

[R13] for 计数循环
来源：http://ave.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://tnl.xylfe.cn

[R14] C 风格 for
来源：http://niw.ydjk.org.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://byq.gotoacloud.top

[R15] while 逐行读文件
来源：http://npl.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ljl.nanxinkj.top

[R16] until 等待条件
来源：http://ryn.andypj.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wqe.fktsv.cn

[R17] 数组定义与取值
来源：http://xrn.sxryk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nib.52xcode.cn

[R18] 遍历数组
来源：http://wmx.havefunace.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wau.xziqi.cn

[R19] 数组长度
来源：http://tuo.vehdjk.com

echo "${#arr[@]}"
来源：http://vws.cheryme.top

[R20] 关联数组（字典）
来源：http://teo.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dqg.dashuyun.cn

[R21] 字符串长度
来源：http://kth.ctjpmb.com

echo "${#s}"
来源：http://cot.fzhhl.top

[R22] 截取子串
来源：http://llg.sxryk.cn

echo "${s:0:5}"
来源：http://fnz.haohaochexian.top

[R23] 字符串替换
来源：http://ujx.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tez.andypj.xyz

[R24] 大小写转换
来源：http://ggf.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://grb.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://kpt.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ing.ywan-chungtsiang.top

[R26] 命令替换
来源：http://gst.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://mox.aizwys.cn

[R27] 算术展开
来源：http://mew.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://vbd.ydzc1.top

[R28] 浮点运算
来源：http://uru.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://nxx.52xcode.cn

[R29] 定义函数
来源：http://lbt.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://een.hysaishi.cn

[R30] 函数返回状态码
来源：http://kyh.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://dcd.haohaochexian.top

[R31] 局部变量
来源：http://yrv.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://cka.hcnkem.com

[R32] 参数个数校验
来源：http://ypw.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bct.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://ctm.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://anl.tarul.cn

[R34] 退出时清理
来源：http://prv.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://pio.jqgufenzy.top

[R35] 后台执行并等待
来源：http://icy.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qym.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://wgu.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://byr.yj20258.top

[R37] 把输出赋给变量
来源：http://vzx.tianlin.xyz

files=$(ls -1)
来源：http://wry.fktsv.cn

[R38] 管道串联
来源：http://ycy.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://ien.9152youxi.cn

[R39] 重定向标准输出与错误
来源：http://miw.epnwcf.com

cmd > out.log 2>&1
来源：http://gyr.9152youxi.cn

[R40] 追加写日志
来源：http://esj.jianghu66.top

echo "log" >> out.log
来源：http://fgm.zdqjudy.top

[R41] 丢弃输出
来源：http://nnv.jianghu66.top

cmd >/dev/null 2>&1
来源：http://jwg.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://lcz.bjfxy.top

wc -l < a.txt
来源：http://opu.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://olk.hammf.cn

find . -name "*.log" -type f
来源：http://mmy.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://rtt.shanyushiyangtech.top

find . -mtime -7 -type f
来源：http://jyd.zhixingplan.top

[R45] 批量删除
来源：http://kpo.andypj.xyz

find . -name "*.tmp" -delete
来源：http://zcf.shanyushiyangtech.top

[R46] 递归替换文件内容
来源：http://mdv.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ebc.bbcook.cn

[R47] sed 单行替换
来源：http://pnf.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zss.nanxinkj.top

[R48] awk 取指定列
来源：http://pxw.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://dvh.hnxiangtu.top

[R49] awk 带条件
来源：http://ina.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://adc.bjfxy.top

[R50] awk 求和
来源：http://gwq.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://jdx.aizwys.cn

[R51] 排序去重取前几
来源：http://ped.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://pxw.ydjk.org.cn

[R52] 统计行数
来源：http://wws.tianlin.xyz

wc -l a.txt
来源：http://mik.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://mmk.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bku.ppjwa.cn

[R54] 比较两个文件
来源：http://zeu.havefunace.top

diff a.txt b.txt
来源：http://gmy.wangdashe.top

[R55] 压缩与解压
来源：http://nln.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ruh.hcnkem.com

[R56] 远程拷贝
来源：http://pqn.zdqjudy.top

scp file user@host:/path/
来源：http://mwt.jyoumei.cn

[R57] 远程执行命令
来源：http://yxh.smart0.xyz

ssh user@host 'uptime'
来源：http://vmf.yfazqb.com

[R58] 下载文件
来源：http://aum.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wbv.yfazqb.com

[R59] 发 POST JSON
来源：http://tuv.jiagoushi.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cav.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://hwy.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nka.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://bbr.nanxuanxn.top

df -h;  du -sh *
来源：http://bxv.daria6918.cn

[R62] 找最占空间的文件
来源：http://lab.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://jmr.yj20258.top

[R63] 内存与进程
来源：http://ity.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://iha.dianchejie.cn

[R64] 结束进程
来源：http://etc.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://gdu.hammf.cn

[R65] 查看端口占用
来源：http://vqy.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gdq.chenlongwang.top

[R66] 定时任务
来源：http://afg.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://fci.epnwcf.com

[R67] 生成随机十六进制串
来源：http://uvr.birdmap.top

openssl rand -hex 16
来源：http://zmo.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://qkw.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://fhg.jyoumei.cn

[R69] 生成随机密码
来源：http://srf.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://trj.ctjpmb.com

[R70] 时间戳与互转
来源：http://ezf.quarkkingdee.top

date +%s;  date -d @1700000000
来源：http://vwk.epnwcf.com

[R71] 日期格式化
来源：http://rtf.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rwy.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://qpt.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://aut.ybcxt.top

[R73] 分割大日志
来源：http://rkn.jlsjyb.cn

split -l 1000 big.log part_
来源：http://sls.hesvh.cn

[R74] 批量重命名
来源：http://mqa.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gpk.ybcxt.top

[R75] 导出环境变量
来源：http://ido.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://why.c1oappe.top

[R76] 使用临时文件
来源：http://gcj.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cpa.yangfankeji.com

[R77] 读取用户输入
来源：http://szd.havefunace.top

read -rp "请输入: " ans
来源：http://ddx.fzhhl.top

[R78] 交互式菜单
来源：http://wga.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://aag.ctjpmb.com

[R79] 解析命令行选项
来源：http://fhr.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rxb.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://ibf.xuanzx.com

time ./run.sh
来源：http://bej.sweek.top

================================================================================
来源：http://xmi.fanxiaobao.xyz

S. C / C++ 专题
来源：http://bkf.fktsv.cn

================================================================================
来源：http://lsw.yanxiufei.cn

[S01] C：Hello World
来源：http://rxz.nanxuanxn.top

#include <stdio.h>
来源：http://now.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bch.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://ikt.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://ohs.pengpengdd.cyou

[S03] C：读入整数
来源：http://sfo.gzhubu.top

int x; scanf("%d", &x);
来源：http://slc.cqqwz.cn

[S04] C：字符串复制
来源：http://nkz.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://kkd.xinyue.icu

[S05] C：字符串长度
来源：http://itl.yueranfly.top

strlen(s)
来源：http://jvm.zhengqikj.top

[S06] C：字符串比较
来源：http://klk.gaohongyu789.top

strcmp(a, b) == 0
来源：http://zpc.0kj1m.cn

[S07] C：数组遍历求和
来源：http://nkg.yj20258.top


<!-- 参考信息 -->