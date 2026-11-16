代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://fuc.jinghuilouyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mhr.jiagoushi.top

[Q43] 标量子查询
来源：http://gho.bjfxy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uvx.ydzc1.top

[Q44] IN 子查询
来源：http://vij.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ysy.dianchejie.cn

[Q45] EXISTS 判断存在
来源：http://wnu.xinyue.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fgx.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zmh.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zpm.fengsongda.top

[Q47] 与平均值比较
来源：http://wxd.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nil.andypj.xyz

[Q48] CTE 公用表表达式
来源：http://ojx.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mhs.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://wgr.tianlin.xyz

[Q49] 更新单行
来源：http://mxy.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ozn.yuxming.cn

[Q50] 批量更新
来源：http://ozv.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fiu.gaohongyu789.top

[Q51] 用子查询更新
来源：http://gcs.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zwf.yueranfly.top

[Q52] 删除指定行
来源：http://kyx.jianghu66.top

DELETE FROM users WHERE id = 10;
来源：http://wvu.hesvh.cn

[Q53] 按条件删除
来源：http://fvq.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rjt.dashuyun.cn

[Q54] 清空表
来源：http://hob.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://clw.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://ttj.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kbc.shanyushiyangtech.top

[Q56] 密集排名（并列不占位）
来源：http://uxx.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://frv.zhijiandao.cn

[Q57] 行号
来源：http://bss.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jik.gaohongyu789.top

[Q58] 累计求和
来源：http://mms.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qge.aibaodan.cn

[Q59] 分组内累计
来源：http://ypp.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yyo.ppjwa.cn

[Q60] 取上一行 / 下一行
来源：http://pbp.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fib.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ktw.zhiwuduotai.top

[Q61] 移动平均
来源：http://zwb.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gdv.yj20258888.top

[Q62] 分组占比
来源：http://doh.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fbe.hammf.cn

[Q63] 开启事务
来源：http://zdj.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gjp.hongshengwenyu.top

[Q64] 提交事务
来源：http://wsm.yj20258888.top

COMMIT;
来源：http://yug.svipenyu.cn

[Q65] 回滚事务
来源：http://ugo.yuanzhike.top

ROLLBACK;
来源：http://jdt.hnxiangtu.top

[Q66] 行锁查询
来源：http://nkl.ydzc1.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lno.nwbrower.top

[Q67] 设置隔离级别
来源：http://gah.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fta.yanxiufei.cn

[Q68] 保存点
来源：http://ueb.aizwys.cn

SAVEPOINT sp1;
来源：http://uyr.jiagoushi.top

ROLLBACK TO sp1;
来源：http://ahn.cdnleiting.top

[Q69] 查看执行计划
来源：http://zyp.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zmk.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://hhq.snrcjt.cn

ANALYZE TABLE users;
来源：http://mzp.zhoulong.xyz

[Q71] 查看建表语句
来源：http://icq.zdbjq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nal.kuanghao11.cn

[Q72] 查看索引
来源：http://btr.ctjpmb.com

SHOW INDEX FROM users;
来源：http://ehl.hongshengwenyu.top

[Q73] 查看表状态
来源：http://say.zdqjudy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://iom.shuidangran.top

[Q74] 强制使用索引
来源：http://rst.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ouk.jinqigufen.top

[Q75] 日期格式化
来源：http://rhr.ydjk.org.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nty.tanke756.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aas.ppjwa.cn

[Q76] 按天统计
来源：http://qgm.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://piv.hnqzz.top

[Q77] 时间加减
来源：http://lny.zhijiandao.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zoc.aibaodan.cn

[Q78] 当前时间
来源：http://hzd.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tvo.yonumen.top

[Q79] 字符串拼接
来源：http://ytz.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hmi.yj20258.top

[Q80] 字符串截取
来源：http://bna.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pvi.yj20258.top

[Q81] 字符串替换
来源：http://ogt.ydjk.org.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ztu.havefunace.top

[Q82] 字符长度与字节长度
来源：http://nik.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xci.yuanzhike.top

[Q83] 大小写转换
来源：http://dty.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://drf.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://vsp.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://apz.zdqjudy.top

[Q85] 数值取整
来源：http://vmf.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://loa.zhoulong.xyz

[Q86] 读取 JSON 字段
来源：http://kvh.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bui.xuetiantiany.cn

[Q87] JSON 字段做条件
来源：http://hsz.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://drq.jinghuilouyu.cn

[Q88] 行转列（条件聚合）
来源：http://jcl.zhengqikj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://muv.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mqj.xylfe.cn

[Q89] 判断表是否存在
来源：http://ozg.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rzz.cucudq.cn

[Q90] 生成序号列
来源：http://fck.yj20258888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xfz.cqqwz.cn

================================================================================
来源：http://ghm.shzxlz.cn

R. Bash 专题
来源：http://utc.ydzc1.top

================================================================================
来源：http://oed.yuanzhike.top

[R01] shebang 与严格模式
来源：http://pki.316326.xyz

#!/usr/bin/env bash
来源：http://jio.cucudq.cn

set -euo pipefail
来源：http://ckt.gogol.net.cn

[R02] 变量赋值与使用
来源：http://bnm.quarkkingdee.top

name="Tom"; echo "$name"
来源：http://hoe.52xcode.cn

[R03] 只读变量
来源：http://eft.tian-w.cn

readonly PI=3.14
来源：http://yop.52xcode.cn

[R04] 位置参数
来源：http://ibv.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mmr.cqqwz.cn

[R05] 参数默认值
来源：http://jtd.nanxuanxn.top

name="${1:-default}"
来源：http://nxq.sweek.top

[R06] 判断命令是否存在
来源：http://vxa.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vfn.aibaodan.cn

[R07] if 判断文件
来源：http://vpl.shanyushiyangtech.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://puu.jinyuanbaomall.cn

[R08] 数值比较
来源：http://fou.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xgd.yangfankeji.com

[R09] 字符串比较
来源：http://ugc.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ssx.svipenyu.cn

[R10] 正则匹配
来源：http://qvu.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xkj.haohaochexian.top

[R11] case 多分支
来源：http://ykx.chenlongwang.top

case "$1" in
来源：http://onq.nwbrower.top

start) echo "启动" ;;
来源：http://nux.ydzc1.top

stop)  echo "停止" ;;
来源：http://knm.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://lls.hnxiangtu.top

esac
来源：http://rmr.nwbrower.top

[R12] for 遍历文件
来源：http://gdr.ydjk.org.cn

for f in *.txt; do echo "$f"; done
来源：http://jtk.fzhhl.top

[R13] for 计数循环
来源：http://ari.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://znm.jqgfzy.top

[R14] C 风格 for
来源：http://dkl.yangfankeji.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ihq.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://prt.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oyx.dianchejie.cn

[R16] until 等待条件
来源：http://ocr.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kbt.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://omx.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://bkm.guannengcc.top

[R18] 遍历数组
来源：http://ogm.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fhf.jianghu66.top

[R19] 数组长度
来源：http://hlm.zhixingplan.top

echo "${#arr[@]}"
来源：http://upa.uphjek.com

[R20] 关联数组（字典）
来源：http://amu.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xig.zhaomingkeji.xyz

[R21] 字符串长度
来源：http://rdc.yonumen.top

echo "${#s}"
来源：http://wnr.hnqzz.top

[R22] 截取子串
来源：http://rjl.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://ocz.pycfn.com

[R23] 字符串替换
来源：http://fua.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nza.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://alu.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vfq.jqgufenzy.top

[R25] 去后缀 / 去前缀
来源：http://qfg.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fwe.hywenlv.cn

[R26] 命令替换
来源：http://sku.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://fis.fanxiaobao.xyz

[R27] 算术展开
来源：http://pjg.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://wep.ppjwa.cn

[R28] 浮点运算
来源：http://ztj.zycfv.cn

echo "scale=2; 10/3" | bc
来源：http://hfa.feifeiyinyue.top

[R29] 定义函数
来源：http://wsw.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qjz.birdmap.top

[R30] 函数返回状态码
来源：http://pof.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://cjd.svipenyu.cn

[R31] 局部变量
来源：http://xfn.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://kzl.ppjwa.cn

[R32] 参数个数校验
来源：http://boz.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gxi.zdqjudy.top

[R33] 捕获错误并提示行号
来源：http://vjl.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cuj.gotoacloud.top

[R34] 退出时清理
来源：http://dem.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://zot.sufxvd.cn

[R35] 后台执行并等待
来源：http://vzm.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ezs.shanyushiyangtech.top

[R36] 并发执行多个任务
来源：http://ebj.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nqa.zycfv.cn

[R37] 把输出赋给变量
来源：http://slp.daria6918.cn

files=$(ls -1)
来源：http://arc.xylfe.cn

[R38] 管道串联
来源：http://pgy.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://pvb.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://mas.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://ktu.zycfv.cn

[R40] 追加写日志
来源：http://eio.shanyushiyangtech.top

echo "log" >> out.log
来源：http://qyx.sxryk.cn

[R41] 丢弃输出
来源：http://gqx.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://kts.52xcode.cn

[R42] 输入重定向
来源：http://umz.hfpthk.cn

wc -l < a.txt
来源：http://dbw.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://tvj.yvedp.cn

find . -name "*.log" -type f
来源：http://yiq.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://mrh.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://rav.zhengqikj.top

[R45] 批量删除
来源：http://htm.jinqigfzy.top

find . -name "*.tmp" -delete
来源：http://nyz.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://emx.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rcv.zhengqikj.top

[R47] sed 单行替换
来源：http://mtc.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://mmu.cheryme.top

[R48] awk 取指定列
来源：http://kca.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://ujn.bjfxy.top

[R49] awk 带条件
来源：http://vdl.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uvq.meibo888.top

[R50] awk 求和
来源：http://efp.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://hek.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://pcw.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wlm.ppjwa.cn

[R52] 统计行数
来源：http://ley.kuanghao11.cn

wc -l a.txt
来源：http://qvn.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://uho.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jhk.ppjwa.cn

[R54] 比较两个文件
来源：http://bih.sjlbkw.cn

diff a.txt b.txt
来源：http://arl.zhoulong.xyz

[R55] 压缩与解压
来源：http://gvu.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xpt.xinyue.icu

[R56] 远程拷贝
来源：http://mvs.sxryk.cn

scp file user@host:/path/
来源：http://uqb.redwolf501.top

[R57] 远程执行命令
来源：http://jmk.zhijiandao.cn

ssh user@host 'uptime'
来源：http://zym.shuidangran.top

[R58] 下载文件
来源：http://lgf.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wgf.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://tja.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jtv.ivvv.top

[R60] 只看 HTTP 状态码
来源：http://pto.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qdo.9152youxi.cn

[R61] 磁盘占用
来源：http://itv.smart0.xyz

df -h;  du -sh *
来源：http://jgl.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://iyc.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://fzr.zhoulong.xyz

[R63] 内存与进程
来源：http://ciz.tarul.cn

free -h;  ps aux | grep nginx
来源：http://wfh.zdqjudy.top

[R64] 结束进程
来源：http://imb.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://zwl.316326.xyz

[R65] 查看端口占用
来源：http://qos.daxiang520.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lvb.sufxvd.cn

[R66] 定时任务
来源：http://xlt.ydjk.org.cn

crontab -e;  crontab -l
来源：http://klc.fengsongda.top

[R67] 生成随机十六进制串
来源：http://wvq.havefunace.top

openssl rand -hex 16
来源：http://soq.cashguo.top

[R68] 计算文件校验值
来源：http://qgb.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://ptv.zhijiandao.cn

[R69] 生成随机密码
来源：http://rrz.gzhubu.top

head -c 16 /dev/urandom | base64
来源：http://qxx.c1oappe.top

[R70] 时间戳与互转
来源：http://sne.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://pkf.zhiwuduotai.top

[R71] 日期格式化
来源：http://lec.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bwo.xylfe.cn

[R72] 等待端口就绪
来源：http://tza.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://znv.zdbjq.cn

[R73] 分割大日志
来源：http://ghw.uphjek.com

split -l 1000 big.log part_
来源：http://vfl.pengpengdd.cyou

[R74] 批量重命名
来源：http://ama.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tex.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://ytx.cashguo.top

export PATH="$HOME/bin:$PATH"
来源：http://ude.xziqi.cn

[R76] 使用临时文件
来源：http://sej.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dur.xuanzx.com

[R77] 读取用户输入
来源：http://oyy.ybcxt.top

read -rp "请输入: " ans
来源：http://wny.cheryme.top

[R78] 交互式菜单
来源：http://yal.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fkc.fengsongda.top

[R79] 解析命令行选项
来源：http://dpi.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://olj.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://avl.gotoacloud.top

time ./run.sh
来源：http://coo.iojbl.cn

================================================================================
来源：http://syp.yangfankeji.com

S. C / C++ 专题
来源：http://wif.sweek.top

================================================================================
来源：http://qrl.hnxiangtu.top

[S01] C：Hello World
来源：http://ugj.316326.xyz

#include <stdio.h>
来源：http://ipq.xuetiantiany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wwb.ybcxt.top

[S02] C：变量与格式化输出
来源：http://mrn.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://dpi.hnxiangtu.top

[S03] C：读入整数
来源：http://rjv.yfazqb.com

int x; scanf("%d", &x);
来源：http://awh.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://vvo.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://bvh.nanxinkj.top

[S05] C：字符串长度
来源：http://kwj.aizwys.cn

strlen(s)
来源：http://zbk.shuidangran.top

[S06] C：字符串比较
来源：http://wou.vqdsnc.cn

strcmp(a, b) == 0
来源：http://qyl.zhengqikj.top

[S07] C：数组遍历求和
来源：http://bkg.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qrh.daxiang520.top

[S08] C：动态内存分配与释放
来源：http://pkl.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lae.cucudq.cn

[S09] C：结构体定义与初始化
来源：http://bds.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hmu.hesvh.cn

[S10] C：指针与解引用
来源：http://xib.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://izx.9152youxi.cn

[S11] C：逐行读文件
来源：http://zym.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://hlj.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xyu.chenlongwang.top

fclose(f);
来源：http://llx.ppjwa.cn

[S12] C：写文件
来源：http://jiz.shzxlz.cn


<!-- 参考信息 -->