代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://peb.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bzy.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dxu.epnwcf.com

[Q41] 多表连接
来源：http://osg.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gnt.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://oqd.aibaodan.cn

JOIN products p ON p.id = o.product_id;
来源：http://xju.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://mik.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://rzf.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nrs.ivvv.top

[Q43] 标量子查询
来源：http://ici.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wll.zhongyouzk.top

[Q44] IN 子查询
来源：http://rrx.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dfy.meibo888.top

[Q45] EXISTS 判断存在
来源：http://wxc.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vxz.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://izn.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lci.zdbjq.cn

[Q47] 与平均值比较
来源：http://fwg.jinqigfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ozm.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://vzv.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xtr.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://hol.shanyushiyangtech.top

[Q49] 更新单行
来源：http://dvb.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bwx.birdmap.top

[Q50] 批量更新
来源：http://zdq.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dhl.bjfxy.top

[Q51] 用子查询更新
来源：http://ozi.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uny.cashguo.top

[Q52] 删除指定行
来源：http://wpk.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://ike.nanxinkj.top

[Q53] 按条件删除
来源：http://lok.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hzd.iojbl.cn

[Q54] 清空表
来源：http://pqy.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://mnv.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://our.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://btt.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://cyr.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fil.nanxuanxn.top

[Q57] 行号
来源：http://ofo.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hqx.gotoacloud.top

[Q58] 累计求和
来源：http://ysq.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vjc.vqdsnc.cn

[Q59] 分组内累计
来源：http://ntg.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ljt.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://pha.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iap.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://idg.uphjek.com

[Q61] 移动平均
来源：http://lfn.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sdc.tianlin.xyz

[Q62] 分组占比
来源：http://ikc.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sat.nanxinkj.top

[Q63] 开启事务
来源：http://mcl.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://smb.cucudq.cn

[Q64] 提交事务
来源：http://pva.zhoulong.xyz

COMMIT;
来源：http://vat.feifeiyinyue.top

[Q65] 回滚事务
来源：http://mnd.shanyushiyangkeji.top

ROLLBACK;
来源：http://dme.hywenlv.cn

[Q66] 行锁查询
来源：http://cog.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://asr.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://fdy.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rrm.ivvv.top

[Q68] 保存点
来源：http://etn.zdqjudy.top

SAVEPOINT sp1;
来源：http://xmy.jianghu66.top

ROLLBACK TO sp1;
来源：http://kqs.ydzc1.top

[Q69] 查看执行计划
来源：http://hba.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ruy.ehwqpu.com

[Q70] 更新统计信息
来源：http://cba.svipenyu.cn

ANALYZE TABLE users;
来源：http://nrp.0kj1m.cn

[Q71] 查看建表语句
来源：http://zqo.havefunace.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lic.yfazqb.com

[Q72] 查看索引
来源：http://vev.hcnkem.com

SHOW INDEX FROM users;
来源：http://dqh.hcnkem.com

[Q73] 查看表状态
来源：http://xrf.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://elx.zhixingplan.top

[Q74] 强制使用索引
来源：http://hwi.yangfankeji.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zwu.vehdjk.com

[Q75] 日期格式化
来源：http://rzn.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dew.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://usx.fktsv.cn

[Q76] 按天统计
来源：http://ozu.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ubj.cheryme.top

[Q77] 时间加减
来源：http://nay.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qto.hongshengwenyu.top

[Q78] 当前时间
来源：http://gwt.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gta.kuanghao11.cn

[Q79] 字符串拼接
来源：http://qyh.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sqs.chenzaomai.com

[Q80] 字符串截取
来源：http://hnr.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kkv.cashguo.top

[Q81] 字符串替换
来源：http://hkf.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wzi.mhx1999.top

[Q82] 字符长度与字节长度
来源：http://zlu.kuanghao11.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wee.yonumen.top

[Q83] 大小写转换
来源：http://bvh.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sfq.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://mcn.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://hil.0kj1m.cn

[Q85] 数值取整
来源：http://dze.jyoumei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nhz.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://xmo.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://igi.xuetiantiany.cn

[Q87] JSON 字段做条件
来源：http://dne.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cjq.zdqjudy.top

[Q88] 行转列（条件聚合）
来源：http://kua.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://etq.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pyo.daria6918.cn

[Q89] 判断表是否存在
来源：http://zru.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jrl.hysaishi.cn

[Q90] 生成序号列
来源：http://itn.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://efj.jyoumei.cn

================================================================================
来源：http://flv.sweek.top

R. Bash 专题
来源：http://dvj.jinghuilouyu.cn

================================================================================
来源：http://rze.jqgfzy.top

[R01] shebang 与严格模式
来源：http://ydg.cucudq.cn

#!/usr/bin/env bash
来源：http://fnl.dashuyun.cn

set -euo pipefail
来源：http://mmu.fzhhl.top

[R02] 变量赋值与使用
来源：http://vxz.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://fed.fanxiaobao.xyz

[R03] 只读变量
来源：http://aqz.chenjidiqi.icu

readonly PI=3.14
来源：http://rfe.bbcook.cn

[R04] 位置参数
来源：http://byw.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ehm.hcnkem.com

[R05] 参数默认值
来源：http://mnc.mhx1999.top

name="${1:-default}"
来源：http://mfq.cashguo.top

[R06] 判断命令是否存在
来源：http://jwv.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hme.andypj.xyz

[R07] if 判断文件
来源：http://kot.hnqzz.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jwp.hammf.cn

[R08] 数值比较
来源：http://vhp.redwolf501.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mif.jinghuilouyu.cn

[R09] 字符串比较
来源：http://gkz.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hyp.hammf.cn

[R10] 正则匹配
来源：http://xpi.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qxt.shanyushiyangtech.top

[R11] case 多分支
来源：http://azx.ydzc1.top

case "$1" in
来源：http://ygv.hysaishi.cn

start) echo "启动" ;;
来源：http://dvf.fengsongda.top

stop)  echo "停止" ;;
来源：http://xvv.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://fke.gogol.net.cn

esac
来源：http://sfj.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://art.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://ods.redwolf501.top

[R13] for 计数循环
来源：http://wts.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://quq.aizwys.cn

[R14] C 风格 for
来源：http://rln.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kfc.jinqigfzy.top

[R15] while 逐行读文件
来源：http://kfx.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tgo.hammf.cn

[R16] until 等待条件
来源：http://wtk.hysaishi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jzv.aizwys.cn

[R17] 数组定义与取值
来源：http://zfx.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jxg.andypj.xyz

[R18] 遍历数组
来源：http://upg.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ail.zhixingplan.top

[R19] 数组长度
来源：http://lja.jqgfzy.top

echo "${#arr[@]}"
来源：http://sup.iojbl.cn

[R20] 关联数组（字典）
来源：http://pdi.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ais.mhx1999.top

[R21] 字符串长度
来源：http://hvj.zhengqikj.top

echo "${#s}"
来源：http://dfl.quarkkingdee.top

[R22] 截取子串
来源：http://mko.hnxiangtu.top

echo "${s:0:5}"
来源：http://qtj.havefunace.top

[R23] 字符串替换
来源：http://imk.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fjq.shangyingyoupin.top

[R24] 大小写转换
来源：http://tbx.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://oax.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://oco.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zsk.yfazqb.com

[R26] 命令替换
来源：http://iyy.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://sol.redwolf501.top

[R27] 算术展开
来源：http://fdr.uphjek.com

echo $((1 + 2 * 3))
来源：http://fwj.bjfxy.top

[R28] 浮点运算
来源：http://dsd.zhongyouzk.top

echo "scale=2; 10/3" | bc
来源：http://jka.sxryk.cn

[R29] 定义函数
来源：http://kwa.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://osd.guowangkeji.top

[R30] 函数返回状态码
来源：http://eco.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://xix.snrcjt.cn

[R31] 局部变量
来源：http://zpp.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://euz.tianlin.xyz

[R32] 参数个数校验
来源：http://btw.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vej.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://aad.yj20258888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gds.316326.xyz

[R34] 退出时清理
来源：http://fjs.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://zli.fengsongda.top

[R35] 后台执行并等待
来源：http://ywh.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xxr.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://rjz.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xud.nwbrower.top

[R37] 把输出赋给变量
来源：http://npn.xingfuxueyuan.xyz

files=$(ls -1)
来源：http://omh.aizwys.cn

[R38] 管道串联
来源：http://xtj.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://zod.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://uqs.quarkkingdee.top

cmd > out.log 2>&1
来源：http://czu.hnqzz.top

[R40] 追加写日志
来源：http://zpd.bbcook.cn

echo "log" >> out.log
来源：http://twy.haohaochexian.top

[R41] 丢弃输出
来源：http://som.52xcode.cn

cmd >/dev/null 2>&1
来源：http://twc.hesvh.cn

[R42] 输入重定向
来源：http://qjp.dashuyun.cn

wc -l < a.txt
来源：http://yqi.hesvh.cn

[R43] 按名字查找文件
来源：http://twp.zhengqikj.top

find . -name "*.log" -type f
来源：http://ciq.bbcook.cn

[R44] 按修改时间查找
来源：http://ocm.birdmap.top

find . -mtime -7 -type f
来源：http://cqz.xuanzx.com

[R45] 批量删除
来源：http://klp.zycfv.cn

find . -name "*.tmp" -delete
来源：http://zjn.zhengqikj.top

[R46] 递归替换文件内容
来源：http://ozq.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rod.fzhhl.top

[R47] sed 单行替换
来源：http://sfj.meibo888.top

sed -i 's/foo/bar/g' a.txt
来源：http://oas.gotoacloud.top

[R48] awk 取指定列
来源：http://fvp.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://czu.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://fhi.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xtq.ppjwa.cn

[R50] awk 求和
来源：http://mla.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qkk.haohaochexian.top

[R51] 排序去重取前几
来源：http://xhc.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dxh.xinyue.icu

[R52] 统计行数
来源：http://meo.cqqwz.cn

wc -l a.txt
来源：http://gtl.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://zyi.zdqjudy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yxy.xylfe.cn

[R54] 比较两个文件
来源：http://poy.redwolf501.top

diff a.txt b.txt
来源：http://dvw.pycfn.com

[R55] 压缩与解压
来源：http://pes.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bjb.gotoacloud.top

[R56] 远程拷贝
来源：http://mwc.hnxiangtu.top

scp file user@host:/path/
来源：http://cdi.meibo888.top

[R57] 远程执行命令
来源：http://zlj.cqqwz.cn

ssh user@host 'uptime'
来源：http://fam.yonumen.top

[R58] 下载文件
来源：http://bai.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fok.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://adj.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nxl.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://vzd.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bdo.pycfn.com

[R61] 磁盘占用
来源：http://rjx.birdmap.top

df -h;  du -sh *
来源：http://kwu.xinyue.icu

[R62] 找最占空间的文件
来源：http://neq.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://bth.jinyuanbaomall.cn

[R63] 内存与进程
来源：http://uhe.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://ddw.shuidangran.top

[R64] 结束进程
来源：http://jcw.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://met.xuanzx.com

[R65] 查看端口占用
来源：http://gvr.jlsjyb.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wkd.snrcjt.cn

[R66] 定时任务
来源：http://njp.cqqwz.cn

crontab -e;  crontab -l
来源：http://pde.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://reu.shuidangran.top

openssl rand -hex 16
来源：http://hgh.dianchejie.cn

[R68] 计算文件校验值
来源：http://mfb.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://pxg.hnxiangtu.top

[R69] 生成随机密码
来源：http://btl.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://kvg.yangfankeji.com

[R70] 时间戳与互转
来源：http://lcd.jianghu66.top

date +%s;  date -d @1700000000
来源：http://xyy.yonumen.top

[R71] 日期格式化
来源：http://bhj.zycfv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://umi.svipenyu.cn

[R72] 等待端口就绪
来源：http://vox.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iul.yj202588.top

[R73] 分割大日志
来源：http://fqj.dianchejie.cn

split -l 1000 big.log part_
来源：http://lil.vqdsnc.cn

[R74] 批量重命名
来源：http://owu.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ldo.hammf.cn

[R75] 导出环境变量
来源：http://yil.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://gvx.hnqzz.top

[R76] 使用临时文件
来源：http://fzo.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ahx.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://dua.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://qhq.0kj1m.cn

[R78] 交互式菜单
来源：http://wno.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wgf.yj20258.top

[R79] 解析命令行选项
来源：http://fwq.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ekt.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://zjq.aibaodan.cn

time ./run.sh
来源：http://pud.cqqwz.cn

================================================================================
来源：http://dnx.jlsjyb.cn

S. C / C++ 专题
来源：http://oso.tarul.cn

================================================================================
来源：http://zfa.nanxinkj.top

[S01] C：Hello World
来源：http://cxq.316326.xyz

#include <stdio.h>
来源：http://npu.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://myb.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://zjl.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://tpw.haohaochexian.top

[S03] C：读入整数
来源：http://lua.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://kbb.hammf.cn

[S04] C：字符串复制
来源：http://gxc.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://uuc.dashuyun.cn

[S05] C：字符串长度
来源：http://vot.vqdsnc.cn

strlen(s)
来源：http://hof.andypj.xyz

[S06] C：字符串比较
来源：http://scu.hnxiangtu.top

strcmp(a, b) == 0
来源：http://iiu.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://eyk.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vuo.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://lth.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://afk.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://ykd.gotoacloud.top


<!-- 参考信息 -->