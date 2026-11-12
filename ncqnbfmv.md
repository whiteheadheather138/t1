代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://myt.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cfl.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://jlj.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ywr.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lnn.cucudq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cag.mhx1999.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jud.zdbjq.cn

[Q41] 多表连接
来源：http://wpg.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ykp.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://cwl.yuanzhike.top

JOIN products p ON p.id = o.product_id;
来源：http://nur.cucudq.cn

[Q42] 连接条件附加过滤
来源：http://ojs.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://dao.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ffo.zdqjudy.top

[Q43] 标量子查询
来源：http://tlv.dianchejie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://las.uphjek.com

[Q44] IN 子查询
来源：http://syy.iojbl.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jse.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://wnc.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hka.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://loi.shanyushiyangtech.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ihd.yonumen.top

[Q47] 与平均值比较
来源：http://cmn.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wce.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://hon.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://two.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://fbq.9152youxi.cn

[Q49] 更新单行
来源：http://gme.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rqk.316326.xyz

[Q50] 批量更新
来源：http://ggx.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kjt.xuanzx.com

[Q51] 用子查询更新
来源：http://gvf.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wfa.sjlbkw.cn

[Q52] 删除指定行
来源：http://ruq.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://lrr.hcnkem.com

[Q53] 按条件删除
来源：http://qsz.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mnm.kuanghao11.cn

[Q54] 清空表
来源：http://srk.yuxming.cn

TRUNCATE TABLE logs;
来源：http://rjz.daxiang520.top

[Q55] 排名（并列占位）
来源：http://kfg.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cul.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://cll.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vfm.xinyue.icu

[Q57] 行号
来源：http://cnc.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dik.xuetiantiany.cn

[Q58] 累计求和
来源：http://gds.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fmd.sufxvd.cn

[Q59] 分组内累计
来源：http://lni.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kei.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://aps.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zbq.xinyue.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ylr.meibo888.top

[Q61] 移动平均
来源：http://qld.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cjt.jinqigfzy.top

[Q62] 分组占比
来源：http://dch.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nqx.bbcook.cn

[Q63] 开启事务
来源：http://kcz.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tuk.chenjidiqi.icu

[Q64] 提交事务
来源：http://ywn.mhx1999.top

COMMIT;
来源：http://wja.yj20258.top

[Q65] 回滚事务
来源：http://lwh.zhijiandao.cn

ROLLBACK;
来源：http://pku.feifeiyinyue.top

[Q66] 行锁查询
来源：http://vst.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ebu.xingfuxueyuan.xyz

[Q67] 设置隔离级别
来源：http://zpb.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ieo.meibo888.top

[Q68] 保存点
来源：http://zab.zycfv.cn

SAVEPOINT sp1;
来源：http://urg.guowangkeji.top

ROLLBACK TO sp1;
来源：http://izz.hysaishi.cn

[Q69] 查看执行计划
来源：http://vev.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lgc.9152youxi.cn

[Q70] 更新统计信息
来源：http://rvf.cdnleiting.top

ANALYZE TABLE users;
来源：http://vch.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://crj.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://caz.hesvh.cn

[Q72] 查看索引
来源：http://fan.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://csm.quarkkingdee.top

[Q73] 查看表状态
来源：http://auv.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iio.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://seo.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zua.jinqigufen.top

[Q75] 日期格式化
来源：http://uyy.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kpt.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://etf.hammf.cn

[Q76] 按天统计
来源：http://gew.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://awr.andypj.xyz

[Q77] 时间加减
来源：http://hgt.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ocs.ydjk.org.cn

[Q78] 当前时间
来源：http://mbk.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gbm.svipenyu.cn

[Q79] 字符串拼接
来源：http://wkm.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jmh.zhijiandao.cn

[Q80] 字符串截取
来源：http://opx.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fdp.hesvh.cn

[Q81] 字符串替换
来源：http://jqn.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://alg.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://lul.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eez.gotoacloud.top

[Q83] 大小写转换
来源：http://dlm.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nnm.fengsongda.top

[Q84] 去除首尾空格
来源：http://voo.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://igt.kuanghao11.cn

[Q85] 数值取整
来源：http://iwd.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lte.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://lsp.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hxw.fktsv.cn

[Q87] JSON 字段做条件
来源：http://ojo.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ejx.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://sgg.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lhy.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gmo.ydzc1.top

[Q89] 判断表是否存在
来源：http://iti.shangyingyoupin.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jdo.yj202588.top

[Q90] 生成序号列
来源：http://doe.gotoacloud.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iur.bjfxy.top

================================================================================
来源：http://inu.yj20258888.top

R. Bash 专题
来源：http://lrk.yvedp.cn

================================================================================
来源：http://ovn.zhengqikj.top

[R01] shebang 与严格模式
来源：http://rzz.jianghu66.top

#!/usr/bin/env bash
来源：http://zlr.yvedp.cn

set -euo pipefail
来源：http://rzh.hammf.cn

[R02] 变量赋值与使用
来源：http://ywc.sjlbkw.cn

name="Tom"; echo "$name"
来源：http://oxx.zdqjudy.top

[R03] 只读变量
来源：http://ggx.xuanzx.com

readonly PI=3.14
来源：http://zil.sweek.top

[R04] 位置参数
来源：http://stw.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eiu.tarul.cn

[R05] 参数默认值
来源：http://vdc.epnwcf.com

name="${1:-default}"
来源：http://zpg.zdqjudy.top

[R06] 判断命令是否存在
来源：http://nhw.wangshuangyany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jdj.daxiang520.top

[R07] if 判断文件
来源：http://lae.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wip.xuanzx.com

[R08] 数值比较
来源：http://bru.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tzf.gzhubu.top

[R09] 字符串比较
来源：http://iry.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tpu.redwolf501.top

[R10] 正则匹配
来源：http://piw.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hrx.xuanzx.com

[R11] case 多分支
来源：http://ivt.fehbvm.com

case "$1" in
来源：http://zvf.gaohongyu789.top

start) echo "启动" ;;
来源：http://mye.zhengqikj.top

stop)  echo "停止" ;;
来源：http://tnw.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://oro.cheryme.top

esac
来源：http://zvy.hfpthk.cn

[R12] for 遍历文件
来源：http://nfs.dashuyun.cn

for f in *.txt; do echo "$f"; done
来源：http://zer.52xcode.cn

[R13] for 计数循环
来源：http://wjy.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://qop.gzhubu.top

[R14] C 风格 for
来源：http://jnx.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://odj.xylfe.cn

[R15] while 逐行读文件
来源：http://fef.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ekx.ybcxt.top

[R16] until 等待条件
来源：http://bra.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wzd.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://bxi.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mzd.xziqi.cn

[R18] 遍历数组
来源：http://yvb.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sfp.zhengqikj.top

[R19] 数组长度
来源：http://eaj.wangdashe.top

echo "${#arr[@]}"
来源：http://bft.fzhhl.top

[R20] 关联数组（字典）
来源：http://kxn.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://btj.yfazqb.com

[R21] 字符串长度
来源：http://tti.sweek.top

echo "${#s}"
来源：http://xnd.haohaochexian.top

[R22] 截取子串
来源：http://obr.vqdsnc.cn

echo "${s:0:5}"
来源：http://xid.hnxiangtu.top

[R23] 字符串替换
来源：http://rwi.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fig.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://cih.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pmu.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://ldp.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zaa.gaohongyu789.top

[R26] 命令替换
来源：http://wny.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://wlz.fktsv.cn

[R27] 算术展开
来源：http://kur.wangdashe.top

echo $((1 + 2 * 3))
来源：http://uvj.fehbvm.com

[R28] 浮点运算
来源：http://ngp.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://pla.wangdashe.top

[R29] 定义函数
来源：http://wdq.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vmq.fktsv.cn

[R30] 函数返回状态码
来源：http://xon.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://qno.dashuyun.cn

[R31] 局部变量
来源：http://rse.cashguo.top

f() { local x=1; echo "$x"; }
来源：http://yls.zhengqikj.top

[R32] 参数个数校验
来源：http://guj.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fnj.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://pid.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://irx.cheryme.top

[R34] 退出时清理
来源：http://tin.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://sej.uphjek.com

[R35] 后台执行并等待
来源：http://xkl.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jvt.redwolf501.top

[R36] 并发执行多个任务
来源：http://jyy.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://imx.aizwys.cn

[R37] 把输出赋给变量
来源：http://hoz.xylfe.cn

files=$(ls -1)
来源：http://agp.birdmap.top

[R38] 管道串联
来源：http://jya.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://ono.sweek.top

[R39] 重定向标准输出与错误
来源：http://ech.zhijiandao.cn

cmd > out.log 2>&1
来源：http://ziq.andypj.xyz

[R40] 追加写日志
来源：http://cal.wangshuangyany.cn

echo "log" >> out.log
来源：http://gnf.xuanzx.com

[R41] 丢弃输出
来源：http://dxx.xingfuxueyuan.xyz

cmd >/dev/null 2>&1
来源：http://zbf.nanxinkj.top

[R42] 输入重定向
来源：http://xcj.nanxinkj.top

wc -l < a.txt
来源：http://amu.jqgfzy.top

[R43] 按名字查找文件
来源：http://eua.vehdjk.com

find . -name "*.log" -type f
来源：http://yle.sysykeji.top

[R44] 按修改时间查找
来源：http://tiv.jiagoushi.top

find . -mtime -7 -type f
来源：http://fwq.cashguo.top

[R45] 批量删除
来源：http://hom.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://mcc.vehdjk.com

[R46] 递归替换文件内容
来源：http://fea.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ozc.fzhhl.top

[R47] sed 单行替换
来源：http://seb.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ahl.zhixingplan.top

[R48] awk 取指定列
来源：http://ysk.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://mjh.andypj.xyz

[R49] awk 带条件
来源：http://nus.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ctn.sxryk.cn

[R50] awk 求和
来源：http://kwv.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zeh.aizwys.cn

[R51] 排序去重取前几
来源：http://jgb.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lcw.52xcode.cn

[R52] 统计行数
来源：http://zou.hesvh.cn

wc -l a.txt
来源：http://hfy.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://pjw.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qgx.vqdsnc.cn

[R54] 比较两个文件
来源：http://jir.feifeiyinyue.top

diff a.txt b.txt
来源：http://cgm.sxryk.cn

[R55] 压缩与解压
来源：http://vzq.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://umt.gzhubu.top

[R56] 远程拷贝
来源：http://hqw.jinqigufen.top

scp file user@host:/path/
来源：http://azd.hfpthk.cn

[R57] 远程执行命令
来源：http://vbx.xinyue.icu

ssh user@host 'uptime'
来源：http://xpi.jqgufenzy.top

[R58] 下载文件
来源：http://unq.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kxt.bjfxy.top

[R59] 发 POST JSON
来源：http://wme.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qgl.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://dfb.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://prh.zycfv.cn

[R61] 磁盘占用
来源：http://ejc.cqqwz.cn

df -h;  du -sh *
来源：http://tqz.mhx1999.top

[R62] 找最占空间的文件
来源：http://sgs.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://lnc.yueranfly.top

[R63] 内存与进程
来源：http://uom.cdnleiting.top

free -h;  ps aux | grep nginx
来源：http://yrl.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://qby.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://hga.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://mnz.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nab.gaohongyu789.top

[R66] 定时任务
来源：http://mxi.cashguo.top

crontab -e;  crontab -l
来源：http://nfe.sxryk.cn

[R67] 生成随机十六进制串
来源：http://nfb.andypj.xyz

openssl rand -hex 16
来源：http://bko.zhongyouzk.top

[R68] 计算文件校验值
来源：http://nnz.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://dkq.aibaodan.cn

[R69] 生成随机密码
来源：http://zpk.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://moh.yueranfly.top

[R70] 时间戳与互转
来源：http://zwo.vehdjk.com

date +%s;  date -d @1700000000
来源：http://jbg.chenlongwang.top

[R71] 日期格式化
来源：http://xeg.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qam.316326.xyz

[R72] 等待端口就绪
来源：http://wxf.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://slh.gogol.net.cn

[R73] 分割大日志
来源：http://vno.chenzaomai.com

split -l 1000 big.log part_
来源：http://jbc.tarul.cn

[R74] 批量重命名
来源：http://mur.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zbd.yj20258.top

[R75] 导出环境变量
来源：http://yoa.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://bus.fengsongda.top

[R76] 使用临时文件
来源：http://ixb.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uzy.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://gye.gaohongyu789.top

read -rp "请输入: " ans
来源：http://oty.hesvh.cn

[R78] 交互式菜单
来源：http://zju.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zxp.gotoacloud.top

[R79] 解析命令行选项
来源：http://ajl.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yrl.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://sdv.52xcode.cn

time ./run.sh
来源：http://kkm.gzhubu.top

================================================================================
来源：http://gro.meibo888.top

S. C / C++ 专题
来源：http://woy.jlsjyb.cn

================================================================================
来源：http://cyi.andypj.xyz

[S01] C：Hello World
来源：http://nyv.jinghuilouyu.cn

#include <stdio.h>
来源：http://ati.epnwcf.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://spn.xziqi.cn

[S02] C：变量与格式化输出
来源：http://rra.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://nzp.9152youxi.cn

[S03] C：读入整数
来源：http://wii.sxryk.cn

int x; scanf("%d", &x);
来源：http://lum.ctjpmb.com

[S04] C：字符串复制
来源：http://iev.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://asj.zhijiandao.cn

[S05] C：字符串长度
来源：http://wzp.shuidangran.top

strlen(s)
来源：http://txu.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://usw.zdbjq.cn

strcmp(a, b) == 0
来源：http://mad.nanxinkj.top

[S07] C：数组遍历求和
来源：http://xmt.jyoumei.cn


<!-- 参考信息 -->