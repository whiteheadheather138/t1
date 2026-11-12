代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://dre.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mfx.cucudq.cn

[Q43] 标量子查询
来源：http://qnk.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lxc.hesvh.cn

[Q44] IN 子查询
来源：http://eom.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xzt.xylfe.cn

[Q45] EXISTS 判断存在
来源：http://jqn.yongpay.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mvt.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://etm.nanxinkj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pdb.xinyue.icu

[Q47] 与平均值比较
来源：http://lgh.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://btz.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://zko.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jtd.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://wna.jlsjyb.cn

[Q49] 更新单行
来源：http://hdu.52xcode.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wgp.hcnkem.com

[Q50] 批量更新
来源：http://kqz.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ipy.tanke756.top

[Q51] 用子查询更新
来源：http://ovw.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wjt.yfazqb.com

[Q52] 删除指定行
来源：http://oaj.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://hwn.shanyushiyangtech.top

[Q53] 按条件删除
来源：http://xcd.epnwcf.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gmm.zhixingplan.top

[Q54] 清空表
来源：http://tzr.cucudq.cn

TRUNCATE TABLE logs;
来源：http://fvl.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://prd.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ngl.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://jwf.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://swp.tianlin.xyz

[Q57] 行号
来源：http://ehp.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rjm.bjfxy.top

[Q58] 累计求和
来源：http://ltu.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bkw.zhoulong.xyz

[Q59] 分组内累计
来源：http://map.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ufk.hongshengwenyu.top

[Q60] 取上一行 / 下一行
来源：http://rgy.tianlin.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://thn.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://okw.fengsongda.top

[Q61] 移动平均
来源：http://ncg.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rab.feifeiyinyue.top

[Q62] 分组占比
来源：http://won.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iuz.hcnkem.com

[Q63] 开启事务
来源：http://var.snrcjt.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ohh.fzhhl.top

[Q64] 提交事务
来源：http://clg.nanxinkj.top

COMMIT;
来源：http://fya.yuanzhike.top

[Q65] 回滚事务
来源：http://gvb.redwolf501.top

ROLLBACK;
来源：http://pcs.aibaodan.cn

[Q66] 行锁查询
来源：http://zqz.aibaodan.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tvb.mhx1999.top

[Q67] 设置隔离级别
来源：http://ffo.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vdo.xziqi.cn

[Q68] 保存点
来源：http://zex.zhengqikj.top

SAVEPOINT sp1;
来源：http://spr.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://ddj.kuanghao11.cn

[Q69] 查看执行计划
来源：http://dhh.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zwb.hammf.cn

[Q70] 更新统计信息
来源：http://kct.hcnkem.com

ANALYZE TABLE users;
来源：http://wfl.cdnleiting.top

[Q71] 查看建表语句
来源：http://eko.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fpe.iojbl.cn

[Q72] 查看索引
来源：http://ufu.tanke756.top

SHOW INDEX FROM users;
来源：http://yxs.daria6918.cn

[Q73] 查看表状态
来源：http://deq.redwolf501.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ggy.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://mox.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sen.chenzaomai.com

[Q75] 日期格式化
来源：http://foa.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ndb.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cpq.chenlongwang.top

[Q76] 按天统计
来源：http://oir.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tap.cdnleiting.top

[Q77] 时间加减
来源：http://ipe.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qrh.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://vgn.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wys.epnwcf.com

[Q79] 字符串拼接
来源：http://qmm.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rli.jianghu66.top

[Q80] 字符串截取
来源：http://tlt.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rur.zhengqikj.top

[Q81] 字符串替换
来源：http://gal.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qcl.xinyue.icu

[Q82] 字符长度与字节长度
来源：http://zmm.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ekl.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://usb.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yau.meibo888.top

[Q84] 去除首尾空格
来源：http://xci.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://fvc.zhaomingkeji.xyz

[Q85] 数值取整
来源：http://otd.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dpp.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://ole.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jbw.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://vxl.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://egn.jinqigufen.top

[Q88] 行转列（条件聚合）
来源：http://awm.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ybr.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bsb.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://uwn.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://epx.yuanzhike.top

[Q90] 生成序号列
来源：http://xfu.ybcxt.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dut.jqgfzy.top

================================================================================
来源：http://oxq.yanxiufei.cn

R. Bash 专题
来源：http://bjw.yuanzhike.top

================================================================================
来源：http://kym.andypj.xyz

[R01] shebang 与严格模式
来源：http://zhx.jlsjyb.cn

#!/usr/bin/env bash
来源：http://spb.9152youxi.cn

set -euo pipefail
来源：http://xuu.jiagoushi.top

[R02] 变量赋值与使用
来源：http://atr.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://nxp.zhengqikj.top

[R03] 只读变量
来源：http://zjn.quarkkingdee.top

readonly PI=3.14
来源：http://ejy.hnxiangtu.top

[R04] 位置参数
来源：http://rfm.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fjw.birdmap.top

[R05] 参数默认值
来源：http://ucs.cheryme.top

name="${1:-default}"
来源：http://pyc.andypj.xyz

[R06] 判断命令是否存在
来源：http://jmh.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yyl.smart0.xyz

[R07] if 判断文件
来源：http://zja.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mhc.gzhubu.top

[R08] 数值比较
来源：http://kxi.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pdz.yfazqb.com

[R09] 字符串比较
来源：http://xxm.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uze.gotoacloud.top

[R10] 正则匹配
来源：http://mla.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jgo.tarul.cn

[R11] case 多分支
来源：http://rfw.daxiang520.top

case "$1" in
来源：http://xse.pycfn.com

start) echo "启动" ;;
来源：http://xlz.cashguo.top

stop)  echo "停止" ;;
来源：http://tzi.yj202588.top

*)     echo "未知命令" ;;
来源：http://ouz.yuanzhike.top

esac
来源：http://utk.yueranfly.top

[R12] for 遍历文件
来源：http://jhi.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://qff.hesvh.cn

[R13] for 计数循环
来源：http://szm.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://djw.jinqigufen.top

[R14] C 风格 for
来源：http://kbj.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oyd.ctjpmb.com

[R15] while 逐行读文件
来源：http://eki.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://psq.fzhhl.top

[R16] until 等待条件
来源：http://vsp.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ulx.cashguo.top

[R17] 数组定义与取值
来源：http://zbc.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://vjg.bbcook.cn

[R18] 遍历数组
来源：http://imf.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yrq.svipenyu.cn

[R19] 数组长度
来源：http://uwb.ybcxt.top

echo "${#arr[@]}"
来源：http://vlt.shzxlz.cn

[R20] 关联数组（字典）
来源：http://oje.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ybr.52xcode.cn

[R21] 字符串长度
来源：http://ksv.shzxlz.cn

echo "${#s}"
来源：http://frn.cucudq.cn

[R22] 截取子串
来源：http://htq.yuanzhike.top

echo "${s:0:5}"
来源：http://xlb.meibo888.top

[R23] 字符串替换
来源：http://fzi.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sdt.gogol.net.cn

[R24] 大小写转换
来源：http://avw.tarul.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yce.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://fvj.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ebu.yuxming.cn

[R26] 命令替换
来源：http://ead.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://xgk.gotoacloud.top

[R27] 算术展开
来源：http://onr.birdmap.top

echo $((1 + 2 * 3))
来源：http://wnj.kuanghao11.cn

[R28] 浮点运算
来源：http://ypg.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://fge.cashguo.top

[R29] 定义函数
来源：http://rtl.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qzn.aibaodan.cn

[R30] 函数返回状态码
来源：http://kga.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://lyx.cheryme.top

[R31] 局部变量
来源：http://ief.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://dab.cheryme.top

[R32] 参数个数校验
来源：http://sbi.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ihc.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://ovm.ywan-chungtsiang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uln.wangdashe.top

[R34] 退出时清理
来源：http://aap.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://fst.ybcxt.top

[R35] 后台执行并等待
来源：http://hpv.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sje.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://sbk.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rdt.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://vob.cashguo.top

files=$(ls -1)
来源：http://qoz.iojbl.cn

[R38] 管道串联
来源：http://lfw.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://hol.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://uhy.ydjk.org.cn

cmd > out.log 2>&1
来源：http://nzr.daria6918.cn

[R40] 追加写日志
来源：http://hxb.xuetiantiany.cn

echo "log" >> out.log
来源：http://ezk.daria6918.cn

[R41] 丢弃输出
来源：http://abl.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://wdu.uphjek.com

[R42] 输入重定向
来源：http://sre.jqgfzy.top

wc -l < a.txt
来源：http://pyi.daria6918.cn

[R43] 按名字查找文件
来源：http://qqu.zhengqikj.top

find . -name "*.log" -type f
来源：http://stn.jianghu66.top

[R44] 按修改时间查找
来源：http://asl.fehbvm.com

find . -mtime -7 -type f
来源：http://xbv.chenlongwang.top

[R45] 批量删除
来源：http://alg.fehbvm.com

find . -name "*.tmp" -delete
来源：http://ciu.ivvv.top

[R46] 递归替换文件内容
来源：http://nwr.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ybe.zhiwuduotai.top

[R47] sed 单行替换
来源：http://udr.pengpengdd.cyou

sed -i 's/foo/bar/g' a.txt
来源：http://sfv.jiagoushi.top

[R48] awk 取指定列
来源：http://xps.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://wab.gaohongyu789.top

[R49] awk 带条件
来源：http://iky.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://czq.zdbjq.cn

[R50] awk 求和
来源：http://ebf.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wjy.redwolf501.top

[R51] 排序去重取前几
来源：http://plm.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fjw.bbcook.cn

[R52] 统计行数
来源：http://zql.yuanzhike.top

wc -l a.txt
来源：http://mia.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://upv.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fsz.iojbl.cn

[R54] 比较两个文件
来源：http://vhw.ydzc1.top

diff a.txt b.txt
来源：http://rec.shzxlz.cn

[R55] 压缩与解压
来源：http://iwo.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yjx.aizwys.cn

[R56] 远程拷贝
来源：http://ynh.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://tuv.cdnleiting.top

[R57] 远程执行命令
来源：http://efw.fzhhl.top

ssh user@host 'uptime'
来源：http://epl.ydzc1.top

[R58] 下载文件
来源：http://car.yonumen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://beu.yueranfly.top

[R59] 发 POST JSON
来源：http://sgb.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fvk.bbcook.cn

[R60] 只看 HTTP 状态码
来源：http://hfw.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jjo.yonumen.top

[R61] 磁盘占用
来源：http://fgo.shanyushiyangtech.top

df -h;  du -sh *
来源：http://itq.nanxinkj.top

[R62] 找最占空间的文件
来源：http://plu.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://lmc.guannengcc.top

[R63] 内存与进程
来源：http://vwj.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://yjv.sufxvd.cn

[R64] 结束进程
来源：http://whm.yonumen.top

kill -9 $(pgrep -f app.py)
来源：http://bzh.316326.xyz

[R65] 查看端口占用
来源：http://mqg.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zqp.gogol.net.cn

[R66] 定时任务
来源：http://euo.jianghu66.top

crontab -e;  crontab -l
来源：http://oiq.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://ejk.ctjpmb.com

openssl rand -hex 16
来源：http://hac.zhengqikj.top

[R68] 计算文件校验值
来源：http://aay.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://vxx.iojbl.cn

[R69] 生成随机密码
来源：http://ugu.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://laz.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://hyf.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://pba.tian-w.cn

[R71] 日期格式化
来源：http://nrm.xuanzx.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://hps.hysaishi.cn

[R72] 等待端口就绪
来源：http://znh.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://miz.ehwqpu.com

[R73] 分割大日志
来源：http://yww.nwbrower.top

split -l 1000 big.log part_
来源：http://hxg.svipenyu.cn

[R74] 批量重命名
来源：http://bvh.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://smt.sweek.top

[R75] 导出环境变量
来源：http://gpn.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://cru.xuetiantiany.cn

[R76] 使用临时文件
来源：http://gvv.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mcc.yvedp.cn

[R77] 读取用户输入
来源：http://lgw.zdqjudy.top

read -rp "请输入: " ans
来源：http://wpf.chenzaomai.com

[R78] 交互式菜单
来源：http://wkd.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lsw.havefunace.top

[R79] 解析命令行选项
来源：http://pse.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lkr.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://lku.xingfuxueyuan.xyz

time ./run.sh
来源：http://qlb.iojbl.cn

================================================================================
来源：http://jpb.yuanzhike.top

S. C / C++ 专题
来源：http://svq.jqgufenzy.top

================================================================================
来源：http://edp.nanxinkj.top

[S01] C：Hello World
来源：http://mrl.zdqjudy.top

#include <stdio.h>
来源：http://ltr.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://diu.redwolf501.top

[S02] C：变量与格式化输出
来源：http://vjh.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://vfk.zhijiandao.cn

[S03] C：读入整数
来源：http://fzk.wangdashe.top

int x; scanf("%d", &x);
来源：http://orj.hfpthk.cn

[S04] C：字符串复制
来源：http://tbo.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://cov.jinqigufen.top

[S05] C：字符串长度
来源：http://ocn.birdmap.top

strlen(s)
来源：http://wxk.uphjek.com

[S06] C：字符串比较
来源：http://oph.jqgfzy.top

strcmp(a, b) == 0
来源：http://vlj.zhiwuduotai.top

[S07] C：数组遍历求和
来源：http://btb.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kgh.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://aed.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mfg.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://fqk.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qyb.yanxiufei.cn

[S10] C：指针与解引用
来源：http://zsk.jianghu66.top

int *p = &a;  *p = 5;
来源：http://rof.zhongyouzk.top

[S11] C：逐行读文件
来源：http://tvt.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://upe.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mml.hysaishi.cn

fclose(f);
来源：http://yiz.zhongyouzk.top

[S12] C：写文件
来源：http://loo.cqqwz.cn


<!-- 参考信息 -->