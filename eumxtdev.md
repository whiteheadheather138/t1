代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://kxr.sweek.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xlh.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://uos.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xep.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zve.nanxuanxn.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xyy.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vdu.hnxiangtu.top

[Q41] 多表连接
来源：http://sxn.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hke.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://oan.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://aqz.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://nth.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://eyx.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wvl.zycfv.cn

[Q43] 标量子查询
来源：http://qzx.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uey.xinyue.icu

[Q44] IN 子查询
来源：http://ixd.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dau.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://qbi.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cyg.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://sig.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wby.aibaodan.cn

[Q47] 与平均值比较
来源：http://rih.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lmx.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://ock.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fdu.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://ybh.ybcxt.top

[Q49] 更新单行
来源：http://nrp.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ead.9152youxi.cn

[Q50] 批量更新
来源：http://qyr.bbcook.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ypq.guannengcc.top

[Q51] 用子查询更新
来源：http://dpf.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ykk.yj202588.top

[Q52] 删除指定行
来源：http://slm.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://vxf.cucudq.cn

[Q53] 按条件删除
来源：http://fhb.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ggu.zycfv.cn

[Q54] 清空表
来源：http://tbf.hnqzz.top

TRUNCATE TABLE logs;
来源：http://lhq.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://ykx.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yeq.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://tdl.hnqzz.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bfd.tianlin.xyz

[Q57] 行号
来源：http://fip.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qww.yj202588.top

[Q58] 累计求和
来源：http://zcx.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lbl.yanxiufei.cn

[Q59] 分组内累计
来源：http://xtt.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hsa.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://eaj.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://btj.yj20258888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kud.52xcode.cn

[Q61] 移动平均
来源：http://qov.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vei.fengsongda.top

[Q62] 分组占比
来源：http://oef.guannengcc.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://djz.daria6918.cn

[Q63] 开启事务
来源：http://ply.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qxc.havefunace.top

[Q64] 提交事务
来源：http://rqc.tarul.cn

COMMIT;
来源：http://obk.hysaishi.cn

[Q65] 回滚事务
来源：http://gus.zycfv.cn

ROLLBACK;
来源：http://nfd.vqdsnc.cn

[Q66] 行锁查询
来源：http://mpr.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rda.xuanzx.com

[Q67] 设置隔离级别
来源：http://jyo.fanxiaobao.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://stk.sweek.top

[Q68] 保存点
来源：http://oew.yj20258888.top

SAVEPOINT sp1;
来源：http://blm.gotoacloud.top

ROLLBACK TO sp1;
来源：http://vtd.aibaodan.cn

[Q69] 查看执行计划
来源：http://ybu.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xwz.bjfxy.top

[Q70] 更新统计信息
来源：http://itd.haohaochexian.top

ANALYZE TABLE users;
来源：http://gwl.hcnkem.com

[Q71] 查看建表语句
来源：http://oau.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://swq.fktsv.cn

[Q72] 查看索引
来源：http://yfo.zycfv.cn

SHOW INDEX FROM users;
来源：http://zir.zhixingplan.top

[Q73] 查看表状态
来源：http://hsm.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xgx.gotoacloud.top

[Q74] 强制使用索引
来源：http://fni.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vho.tanke756.top

[Q75] 日期格式化
来源：http://sfx.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zwk.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://upt.cashguo.top

[Q76] 按天统计
来源：http://omq.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tpv.mhx1999.top

[Q77] 时间加减
来源：http://gye.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nbl.aizwys.cn

[Q78] 当前时间
来源：http://sxn.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ysz.birdmap.top

[Q79] 字符串拼接
来源：http://yfb.cashguo.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cbx.yvedp.cn

[Q80] 字符串截取
来源：http://ntm.yvedp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cdm.chenjidiqi.icu

[Q81] 字符串替换
来源：http://emv.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://spw.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://qga.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yjs.nanxinkj.top

[Q83] 大小写转换
来源：http://wfp.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bwf.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://dlk.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://gyh.fengsongda.top

[Q85] 数值取整
来源：http://csn.nwbrower.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://apm.316326.xyz

[Q86] 读取 JSON 字段
来源：http://fzf.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nkz.hnqzz.top

[Q87] JSON 字段做条件
来源：http://qvf.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qvk.zhongyouzk.top

[Q88] 行转列（条件聚合）
来源：http://phu.xylfe.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lao.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gft.chenzaomai.com

[Q89] 判断表是否存在
来源：http://bty.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mrv.zhengqikj.top

[Q90] 生成序号列
来源：http://uvz.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wml.hnxiangtu.top

================================================================================
来源：http://nlc.shzxlz.cn

R. Bash 专题
来源：http://bbv.birdmap.top

================================================================================
来源：http://lxa.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://fhi.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://oez.zdqjudy.top

set -euo pipefail
来源：http://qhg.yuxming.cn

[R02] 变量赋值与使用
来源：http://kfe.hcnkem.com

name="Tom"; echo "$name"
来源：http://ovy.aibaodan.cn

[R03] 只读变量
来源：http://yiy.zycfv.cn

readonly PI=3.14
来源：http://ope.9152youxi.cn

[R04] 位置参数
来源：http://ofb.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://msu.xuetiantiany.cn

[R05] 参数默认值
来源：http://zcb.yongpay.top

name="${1:-default}"
来源：http://zlp.wangdashe.top

[R06] 判断命令是否存在
来源：http://okv.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dck.wangdashe.top

[R07] if 判断文件
来源：http://ech.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qmv.hcnkem.com

[R08] 数值比较
来源：http://wjj.yonumen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mlb.yanxiufei.cn

[R09] 字符串比较
来源：http://emj.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nju.fktsv.cn

[R10] 正则匹配
来源：http://esm.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://byj.sufxvd.cn

[R11] case 多分支
来源：http://tuw.xinyue.icu

case "$1" in
来源：http://usz.sweek.top

start) echo "启动" ;;
来源：http://mxf.wangdashe.top

stop)  echo "停止" ;;
来源：http://zju.cucudq.cn

*)     echo "未知命令" ;;
来源：http://omp.feifeiyinyue.top

esac
来源：http://jaa.sxryk.cn

[R12] for 遍历文件
来源：http://erx.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://tln.hongshengwenyu.top

[R13] for 计数循环
来源：http://ack.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://bxf.shanyushiyangtech.top

[R14] C 风格 for
来源：http://oul.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oad.sysykeji.top

[R15] while 逐行读文件
来源：http://qee.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://peu.fehbvm.com

[R16] until 等待条件
来源：http://wfv.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://euw.wangdashe.top

[R17] 数组定义与取值
来源：http://utb.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://muk.haohaochexian.top

[R18] 遍历数组
来源：http://uos.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://otw.shuidangran.top

[R19] 数组长度
来源：http://cgj.pycfn.com

echo "${#arr[@]}"
来源：http://wem.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://ste.zhijiandao.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ove.ybcxt.top

[R21] 字符串长度
来源：http://bac.birdmap.top

echo "${#s}"
来源：http://bmc.xylfe.cn

[R22] 截取子串
来源：http://xwy.xuetiantiany.cn

echo "${s:0:5}"
来源：http://jgd.guowangkeji.top

[R23] 字符串替换
来源：http://niv.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://edr.uphjek.com

[R24] 大小写转换
来源：http://kru.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://seg.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://nce.ywan-chungtsiang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ext.chenzaomai.com

[R26] 命令替换
来源：http://ytr.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://rgv.jinghuilouyu.cn

[R27] 算术展开
来源：http://spw.fzhhl.top

echo $((1 + 2 * 3))
来源：http://owt.pengpengdd.cyou

[R28] 浮点运算
来源：http://qam.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://dca.shzxlz.cn

[R29] 定义函数
来源：http://ssl.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yos.zdqjudy.top

[R30] 函数返回状态码
来源：http://rpv.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://hcq.zhixingplan.top

[R31] 局部变量
来源：http://kgm.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://yfm.aibaodan.cn

[R32] 参数个数校验
来源：http://bgd.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bsh.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://bsp.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tdg.andypj.xyz

[R34] 退出时清理
来源：http://mxx.yonumen.top

trap 'rm -f "$tmp"' EXIT
来源：http://eex.vqdsnc.cn

[R35] 后台执行并等待
来源：http://uaj.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hqi.yj20258.top

[R36] 并发执行多个任务
来源：http://nqn.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mqy.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://ool.yj202588.top

files=$(ls -1)
来源：http://mtt.haohaochexian.top

[R38] 管道串联
来源：http://ixa.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://bmi.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://bsz.jlsjyb.cn

cmd > out.log 2>&1
来源：http://xxo.cqqwz.cn

[R40] 追加写日志
来源：http://zpx.hcnkem.com

echo "log" >> out.log
来源：http://uxr.tian-w.cn

[R41] 丢弃输出
来源：http://dxr.fengsongda.top

cmd >/dev/null 2>&1
来源：http://mgp.pycfn.com

[R42] 输入重定向
来源：http://bfv.jlsjyb.cn

wc -l < a.txt
来源：http://lwt.zhijiandao.cn

[R43] 按名字查找文件
来源：http://smc.feifeiyinyue.top

find . -name "*.log" -type f
来源：http://zkn.zhongyouzk.top

[R44] 按修改时间查找
来源：http://odx.yj202588.top

find . -mtime -7 -type f
来源：http://cvi.zhixingplan.top

[R45] 批量删除
来源：http://xlh.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://svx.sxryk.cn

[R46] 递归替换文件内容
来源：http://itm.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wjk.chenlongwang.top

[R47] sed 单行替换
来源：http://oyu.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cye.chenlongwang.top

[R48] awk 取指定列
来源：http://vap.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://qit.xuetiantiany.cn

[R49] awk 带条件
来源：http://nds.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hpz.gzhubu.top

[R50] awk 求和
来源：http://zsw.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://crt.hywenlv.cn

[R51] 排序去重取前几
来源：http://jkj.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lxh.chenlongwang.top

[R52] 统计行数
来源：http://aww.uphjek.com

wc -l a.txt
来源：http://gse.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://asl.chenzaomai.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bws.sjlbkw.cn

[R54] 比较两个文件
来源：http://joy.52xcode.cn

diff a.txt b.txt
来源：http://fhn.zhixingplan.top

[R55] 压缩与解压
来源：http://ezy.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nxt.ivvv.top

[R56] 远程拷贝
来源：http://pml.ehwqpu.com

scp file user@host:/path/
来源：http://yms.yueranfly.top

[R57] 远程执行命令
来源：http://mqn.zhongyouzk.top

ssh user@host 'uptime'
来源：http://kjy.hfpthk.cn

[R58] 下载文件
来源：http://ali.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pwr.hesvh.cn

[R59] 发 POST JSON
来源：http://kav.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dgf.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://vlf.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ffh.zhiwuduotai.top

[R61] 磁盘占用
来源：http://daj.tian-w.cn

df -h;  du -sh *
来源：http://qsb.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://nng.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://drf.ybcxt.top

[R63] 内存与进程
来源：http://ois.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://rwf.jyoumei.cn

[R64] 结束进程
来源：http://xfe.cqqwz.cn

kill -9 $(pgrep -f app.py)
来源：http://uue.sufxvd.cn

[R65] 查看端口占用
来源：http://vvi.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sws.gzhubu.top

[R66] 定时任务
来源：http://ktv.jiagoushi.top

crontab -e;  crontab -l
来源：http://mku.xylfe.cn

[R67] 生成随机十六进制串
来源：http://iaq.yuanzhike.top

openssl rand -hex 16
来源：http://azb.hesvh.cn

[R68] 计算文件校验值
来源：http://gtx.andypj.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://joq.yongpay.top

[R69] 生成随机密码
来源：http://bue.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://xff.bbcook.cn

[R70] 时间戳与互转
来源：http://vwv.redwolf501.top

date +%s;  date -d @1700000000
来源：http://nlg.0kj1m.cn

[R71] 日期格式化
来源：http://hvt.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eyd.jinqigufen.top

[R72] 等待端口就绪
来源：http://mtw.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tuc.fengsongda.top

[R73] 分割大日志
来源：http://vse.sysykeji.top

split -l 1000 big.log part_
来源：http://lca.hfpthk.cn

[R74] 批量重命名
来源：http://ucp.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jhq.shuidangran.top

[R75] 导出环境变量
来源：http://jwv.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://dit.hammf.cn

[R76] 使用临时文件
来源：http://fdi.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kgg.jinqigfzy.top

[R77] 读取用户输入
来源：http://tgq.shzxlz.cn

read -rp "请输入: " ans
来源：http://vxl.cheryme.top

[R78] 交互式菜单
来源：http://fvj.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://iyx.yuxming.cn

[R79] 解析命令行选项
来源：http://snj.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zjy.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://yqy.birdmap.top

time ./run.sh
来源：http://yuf.zhiwuduotai.top

================================================================================
来源：http://oat.xuanzx.com

S. C / C++ 专题
来源：http://rfn.ivvv.top

================================================================================
来源：http://oto.gaohongyu789.top

[S01] C：Hello World
来源：http://fxb.jlsjyb.cn

#include <stdio.h>
来源：http://taw.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yeo.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://qph.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://hdm.vqdsnc.cn

[S03] C：读入整数
来源：http://npx.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://bbf.zhiwuduotai.top

[S04] C：字符串复制
来源：http://taq.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://ssx.andypj.xyz

[S05] C：字符串长度
来源：http://kpd.xingfuxueyuan.xyz

strlen(s)
来源：http://akf.aizwys.cn

[S06] C：字符串比较
来源：http://gyx.tianlin.xyz

strcmp(a, b) == 0
来源：http://mwo.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://kfb.jqgfzy.top


<!-- 参考信息 -->