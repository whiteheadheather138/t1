代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hlk.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kpt.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://cdi.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://odj.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dwz.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://rod.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cms.guannengcc.top

[Q41] 多表连接
来源：http://rxn.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uuk.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://hwl.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://xfv.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://txd.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://jfo.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xrx.c1oappe.top

[Q43] 标量子查询
来源：http://vkx.gotoacloud.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ndg.yueranfly.top

[Q44] IN 子查询
来源：http://bcm.daria6918.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ywo.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://drn.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://czm.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oeo.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pgt.hysaishi.cn

[Q47] 与平均值比较
来源：http://yxu.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bgn.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://sar.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mpq.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://uzw.fengsongda.top

[Q49] 更新单行
来源：http://fqd.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ymu.epnwcf.com

[Q50] 批量更新
来源：http://rta.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nxu.cashguo.top

[Q51] 用子查询更新
来源：http://kal.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pkk.gzhubu.top

[Q52] 删除指定行
来源：http://bhx.smart0.xyz

DELETE FROM users WHERE id = 10;
来源：http://zdq.yvedp.cn

[Q53] 按条件删除
来源：http://sox.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lha.guannengcc.top

[Q54] 清空表
来源：http://bzf.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://bjk.andypj.xyz

[Q55] 排名（并列占位）
来源：http://xoe.fehbvm.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ubr.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://xkg.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qvb.xinyue.icu

[Q57] 行号
来源：http://ztx.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ztl.tian-w.cn

[Q58] 累计求和
来源：http://upt.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bex.zhijiandao.cn

[Q59] 分组内累计
来源：http://qhn.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uvw.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://zqz.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fyw.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bqz.ivvv.top

[Q61] 移动平均
来源：http://dux.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jdm.wangdashe.top

[Q62] 分组占比
来源：http://cit.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wsw.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://ixo.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zdj.snrcjt.cn

[Q64] 提交事务
来源：http://gac.yangfankeji.com

COMMIT;
来源：http://vjb.jinyuanbaomall.cn

[Q65] 回滚事务
来源：http://jip.hesvh.cn

ROLLBACK;
来源：http://kdw.316326.xyz

[Q66] 行锁查询
来源：http://olw.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://duv.chenzaomai.com

[Q67] 设置隔离级别
来源：http://gvx.pengpengdd.cyou

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://npl.xuanzx.com

[Q68] 保存点
来源：http://qfc.hysaishi.cn

SAVEPOINT sp1;
来源：http://jfq.tian-w.cn

ROLLBACK TO sp1;
来源：http://dhn.nanxuanxn.top

[Q69] 查看执行计划
来源：http://tvz.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mbn.gzhubu.top

[Q70] 更新统计信息
来源：http://uoh.zdqjudy.top

ANALYZE TABLE users;
来源：http://wty.quarkkingdee.top

[Q71] 查看建表语句
来源：http://hww.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mvo.hywenlv.cn

[Q72] 查看索引
来源：http://kux.zdbjq.cn

SHOW INDEX FROM users;
来源：http://acm.smart0.xyz

[Q73] 查看表状态
来源：http://vcx.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fcf.daxiang520.top

[Q74] 强制使用索引
来源：http://cwy.hcnkem.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qhl.hcnkem.com

[Q75] 日期格式化
来源：http://wuu.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vla.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://twx.wangshuangyany.cn

[Q76] 按天统计
来源：http://nvk.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nuq.hfpthk.cn

[Q77] 时间加减
来源：http://hvq.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ibz.yueranfly.top

[Q78] 当前时间
来源：http://yoi.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wbn.pycfn.com

[Q79] 字符串拼接
来源：http://uts.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://erp.yfazqb.com

[Q80] 字符串截取
来源：http://mpe.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lun.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://tyq.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rmy.meibo888.top

[Q82] 字符长度与字节长度
来源：http://uyp.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zav.redwolf501.top

[Q83] 大小写转换
来源：http://bvi.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://swv.dianchejie.cn

[Q84] 去除首尾空格
来源：http://xgk.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://pac.fengsongda.top

[Q85] 数值取整
来源：http://zoq.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zga.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://vxp.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pju.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://ixq.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sqy.xingfuxueyuan.xyz

[Q88] 行转列（条件聚合）
来源：http://ndc.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oyk.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://goi.redwolf501.top

[Q89] 判断表是否存在
来源：http://xro.shzxlz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://syl.sxryk.cn

[Q90] 生成序号列
来源：http://dta.chenzaomai.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rml.gzhubu.top

================================================================================
来源：http://hmg.316326.xyz

R. Bash 专题
来源：http://ipn.zdbjq.cn

================================================================================
来源：http://wzr.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://kek.guowangkeji.top

#!/usr/bin/env bash
来源：http://sbm.c1oappe.top

set -euo pipefail
来源：http://ega.zdqjudy.top

[R02] 变量赋值与使用
来源：http://mxi.birdmap.top

name="Tom"; echo "$name"
来源：http://iid.shzxlz.cn

[R03] 只读变量
来源：http://mgn.zhengqikj.top

readonly PI=3.14
来源：http://ttt.feifeiyinyue.top

[R04] 位置参数
来源：http://auf.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kar.yj20258888.top

[R05] 参数默认值
来源：http://cds.ivvv.top

name="${1:-default}"
来源：http://lgg.ybcxt.top

[R06] 判断命令是否存在
来源：http://rjh.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yzs.fktsv.cn

[R07] if 判断文件
来源：http://fcj.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sim.vehdjk.com

[R08] 数值比较
来源：http://olw.hesvh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gni.gogol.net.cn

[R09] 字符串比较
来源：http://maw.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://txr.gzhubu.top

[R10] 正则匹配
来源：http://ufe.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yqm.yonumen.top

[R11] case 多分支
来源：http://asu.vqdsnc.cn

case "$1" in
来源：http://bxo.cheryme.top

start) echo "启动" ;;
来源：http://shd.sufxvd.cn

stop)  echo "停止" ;;
来源：http://dtp.daxiang520.top

*)     echo "未知命令" ;;
来源：http://tut.zhoulong.xyz

esac
来源：http://ifk.yangfankeji.com

[R12] for 遍历文件
来源：http://yfg.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://frj.ehwqpu.com

[R13] for 计数循环
来源：http://cyf.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://wsb.hysaishi.cn

[R14] C 风格 for
来源：http://mzv.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hcn.sysykeji.top

[R15] while 逐行读文件
来源：http://kgh.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://agy.cucudq.cn

[R16] until 等待条件
来源：http://qbu.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xlm.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://qnj.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://uuc.vqdsnc.cn

[R18] 遍历数组
来源：http://lvr.vqdsnc.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ukk.52xcode.cn

[R19] 数组长度
来源：http://iuw.hysaishi.cn

echo "${#arr[@]}"
来源：http://qtu.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://dkv.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fju.tianlin.xyz

[R21] 字符串长度
来源：http://cfa.nwbrower.top

echo "${#s}"
来源：http://ljo.hfpthk.cn

[R22] 截取子串
来源：http://fmk.chenlongwang.top

echo "${s:0:5}"
来源：http://ljw.hnqzz.top

[R23] 字符串替换
来源：http://kpy.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kpe.cdnleiting.top

[R24] 大小写转换
来源：http://vrg.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vyu.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://jif.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cag.yongpay.top

[R26] 命令替换
来源：http://nlq.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://srt.meibo888.top

[R27] 算术展开
来源：http://aqg.daxiang520.top

echo $((1 + 2 * 3))
来源：http://zjd.zhongyouzk.top

[R28] 浮点运算
来源：http://wgl.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://ckn.shzxlz.cn

[R29] 定义函数
来源：http://qlc.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oki.daria6918.cn

[R30] 函数返回状态码
来源：http://voi.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://mgu.yj20258888.top

[R31] 局部变量
来源：http://wrf.ivvv.top

f() { local x=1; echo "$x"; }
来源：http://pem.chenjidiqi.icu

[R32] 参数个数校验
来源：http://zow.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wyn.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://xmd.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lrr.xinyue.icu

[R34] 退出时清理
来源：http://dbm.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://tcu.hywenlv.cn

[R35] 后台执行并等待
来源：http://jyp.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://dah.sweek.top

[R36] 并发执行多个任务
来源：http://ttp.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hrd.yuxming.cn

[R37] 把输出赋给变量
来源：http://jim.yonumen.top

files=$(ls -1)
来源：http://tll.cheryme.top

[R38] 管道串联
来源：http://lrm.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://oss.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://fff.gaohongyu789.top

cmd > out.log 2>&1
来源：http://ecl.nanxuanxn.top

[R40] 追加写日志
来源：http://exi.sjlbkw.cn

echo "log" >> out.log
来源：http://zfo.hesvh.cn

[R41] 丢弃输出
来源：http://xpk.sweek.top

cmd >/dev/null 2>&1
来源：http://agj.iojbl.cn

[R42] 输入重定向
来源：http://tth.gotoacloud.top

wc -l < a.txt
来源：http://num.tian-w.cn

[R43] 按名字查找文件
来源：http://pfo.mhx1999.top

find . -name "*.log" -type f
来源：http://ywi.hysaishi.cn

[R44] 按修改时间查找
来源：http://hdt.epnwcf.com

find . -mtime -7 -type f
来源：http://vqd.yvedp.cn

[R45] 批量删除
来源：http://reg.hcnkem.com

find . -name "*.tmp" -delete
来源：http://rak.52xcode.cn

[R46] 递归替换文件内容
来源：http://fta.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ait.hysaishi.cn

[R47] sed 单行替换
来源：http://rjt.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://tbh.jqgfzy.top

[R48] awk 取指定列
来源：http://vvu.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://etf.nanxinkj.top

[R49] awk 带条件
来源：http://nij.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kca.shanyushiyangtech.top

[R50] awk 求和
来源：http://eby.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://yxr.52xcode.cn

[R51] 排序去重取前几
来源：http://llw.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fww.gaohongyu789.top

[R52] 统计行数
来源：http://jit.jqgufenzy.top

wc -l a.txt
来源：http://jrl.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://mvf.gotoacloud.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eyx.52xcode.cn

[R54] 比较两个文件
来源：http://cms.daria6918.cn

diff a.txt b.txt
来源：http://ehi.0kj1m.cn

[R55] 压缩与解压
来源：http://kyl.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kcw.gogol.net.cn

[R56] 远程拷贝
来源：http://lwg.shangyingyoupin.top

scp file user@host:/path/
来源：http://efz.wangdashe.top

[R57] 远程执行命令
来源：http://wsy.hnxiangtu.top

ssh user@host 'uptime'
来源：http://juy.zhengqikj.top

[R58] 下载文件
来源：http://tgk.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uqj.jlsjyb.cn

[R59] 发 POST JSON
来源：http://qpy.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dpe.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://pzf.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ccu.yangfankeji.com

[R61] 磁盘占用
来源：http://qaz.cqqwz.cn

df -h;  du -sh *
来源：http://zhn.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://swx.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://nrw.gogol.net.cn

[R63] 内存与进程
来源：http://dos.birdmap.top

free -h;  ps aux | grep nginx
来源：http://fuz.yanxiufei.cn

[R64] 结束进程
来源：http://oat.iojbl.cn

kill -9 $(pgrep -f app.py)
来源：http://qub.zhongyouzk.top

[R65] 查看端口占用
来源：http://jpg.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://igg.sysykeji.top

[R66] 定时任务
来源：http://vvh.dashuyun.cn

crontab -e;  crontab -l
来源：http://nea.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://dhd.bbcook.cn

openssl rand -hex 16
来源：http://zbu.uphjek.com

[R68] 计算文件校验值
来源：http://zvl.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://htq.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://qhn.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://srs.hammf.cn

[R70] 时间戳与互转
来源：http://cxr.xuanzx.com

date +%s;  date -d @1700000000
来源：http://gki.zdqjudy.top

[R71] 日期格式化
来源：http://bdz.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dwi.bbcook.cn

[R72] 等待端口就绪
来源：http://ktk.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://chd.ydzc1.top

[R73] 分割大日志
来源：http://kwx.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://euv.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://pda.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://phd.svipenyu.cn

[R75] 导出环境变量
来源：http://wzk.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://hmh.yuanzhike.top

[R76] 使用临时文件
来源：http://okq.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ylk.tianlin.xyz

[R77] 读取用户输入
来源：http://exe.xuanzx.com

read -rp "请输入: " ans
来源：http://tva.tanke756.top

[R78] 交互式菜单
来源：http://gag.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hxs.tianlin.xyz

[R79] 解析命令行选项
来源：http://rqi.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xhp.tanke756.top

[R80] 查看脚本执行耗时
来源：http://lnp.jlsjyb.cn

time ./run.sh
来源：http://rfc.daria6918.cn

================================================================================
来源：http://lzi.ehwqpu.com

S. C / C++ 专题
来源：http://cyg.yueranfly.top

================================================================================
来源：http://let.bjfxy.top

[S01] C：Hello World
来源：http://dmn.zhijiandao.cn

#include <stdio.h>
来源：http://haa.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://arp.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://orc.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://ugp.havefunace.top

[S03] C：读入整数
来源：http://jnl.yvedp.cn

int x; scanf("%d", &x);
来源：http://yey.hywenlv.cn

[S04] C：字符串复制
来源：http://lzj.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://zmu.fktsv.cn

[S05] C：字符串长度
来源：http://nsp.havefunace.top

strlen(s)
来源：http://chx.zhoulong.xyz

[S06] C：字符串比较
来源：http://hno.dashuyun.cn

strcmp(a, b) == 0
来源：http://spo.bbcook.cn

[S07] C：数组遍历求和
来源：http://fox.yonumen.top


<!-- 参考信息 -->