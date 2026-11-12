代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://qtg.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eok.smart0.xyz

[Q47] 与平均值比较
来源：http://jqj.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ngl.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://mvp.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://use.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://bew.xuanzx.com

[Q49] 更新单行
来源：http://fxc.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kcb.nanxinkj.top

[Q50] 批量更新
来源：http://wol.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://krc.yj20258.top

[Q51] 用子查询更新
来源：http://wfs.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vea.hammf.cn

[Q52] 删除指定行
来源：http://pfk.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://hoq.tian-w.cn

[Q53] 按条件删除
来源：http://aco.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gkr.daria6918.cn

[Q54] 清空表
来源：http://agl.guannengcc.top

TRUNCATE TABLE logs;
来源：http://oir.hesvh.cn

[Q55] 排名（并列占位）
来源：http://hcb.kuanghao11.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iog.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://glv.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qhq.ehwqpu.com

[Q57] 行号
来源：http://dqz.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ybp.yanxiufei.cn

[Q58] 累计求和
来源：http://yvp.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mts.hcnkem.com

[Q59] 分组内累计
来源：http://slo.xuanzx.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dzb.yuxming.cn

[Q60] 取上一行 / 下一行
来源：http://efq.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jxc.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nlm.hongshengwenyu.top

[Q61] 移动平均
来源：http://ktb.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oga.ybcxt.top

[Q62] 分组占比
来源：http://ywt.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xdw.daria6918.cn

[Q63] 开启事务
来源：http://rlf.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hbt.yueranfly.top

[Q64] 提交事务
来源：http://jvr.tanke756.top

COMMIT;
来源：http://xhy.cqqwz.cn

[Q65] 回滚事务
来源：http://tqd.wangshuangyany.cn

ROLLBACK;
来源：http://xll.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://bav.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aot.guowangkeji.top

[Q67] 设置隔离级别
来源：http://zds.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kwc.tanke756.top

[Q68] 保存点
来源：http://dgj.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://wct.shzxlz.cn

ROLLBACK TO sp1;
来源：http://ycj.xuanzx.com

[Q69] 查看执行计划
来源：http://jvc.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://czj.tarul.cn

[Q70] 更新统计信息
来源：http://oeu.pengpengdd.cyou

ANALYZE TABLE users;
来源：http://jrh.shuidangran.top

[Q71] 查看建表语句
来源：http://mmp.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cpe.chenlongwang.top

[Q72] 查看索引
来源：http://oab.zdbjq.cn

SHOW INDEX FROM users;
来源：http://ovk.ppjwa.cn

[Q73] 查看表状态
来源：http://gfu.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uoj.quarkkingdee.top

[Q74] 强制使用索引
来源：http://pym.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bob.aibaodan.cn

[Q75] 日期格式化
来源：http://lkk.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sxk.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ito.hysaishi.cn

[Q76] 按天统计
来源：http://ovx.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://krk.guowangkeji.top

[Q77] 时间加减
来源：http://hgr.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lze.bbcook.cn

[Q78] 当前时间
来源：http://ejf.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xlu.quarkkingdee.top

[Q79] 字符串拼接
来源：http://qza.yfazqb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oxq.gotoacloud.top

[Q80] 字符串截取
来源：http://rkc.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sgi.haohaochexian.top

[Q81] 字符串替换
来源：http://lev.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ast.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://lio.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xgn.aizwys.cn

[Q83] 大小写转换
来源：http://rpi.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qxd.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://efi.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://qdj.cucudq.cn

[Q85] 数值取整
来源：http://shk.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aat.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://qth.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rkw.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://ueg.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kdz.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://jdl.chenjidiqi.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uem.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hdg.hfpthk.cn

[Q89] 判断表是否存在
来源：http://lyy.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lbw.yuanzhike.top

[Q90] 生成序号列
来源：http://dkn.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xzq.jinyuanbaomall.cn

================================================================================
来源：http://ceg.yangfankeji.com

R. Bash 专题
来源：http://wbr.shangyingyoupin.top

================================================================================
来源：http://jya.gogol.net.cn

[R01] shebang 与严格模式
来源：http://nsi.wangdashe.top

#!/usr/bin/env bash
来源：http://mrh.xuetiantiany.cn

set -euo pipefail
来源：http://fuz.cashguo.top

[R02] 变量赋值与使用
来源：http://koy.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://rgk.hcnkem.com

[R03] 只读变量
来源：http://hhk.iojbl.cn

readonly PI=3.14
来源：http://fhb.yonumen.top

[R04] 位置参数
来源：http://pgr.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://scs.gogol.net.cn

[R05] 参数默认值
来源：http://nkp.daria6918.cn

name="${1:-default}"
来源：http://lbe.c1oappe.top

[R06] 判断命令是否存在
来源：http://apu.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zxp.daria6918.cn

[R07] if 判断文件
来源：http://xfs.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nkp.zhengqikj.top

[R08] 数值比较
来源：http://dlt.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tlw.ehwqpu.com

[R09] 字符串比较
来源：http://uje.uphjek.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://swv.cqqwz.cn

[R10] 正则匹配
来源：http://ene.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jok.wangshuangyany.cn

[R11] case 多分支
来源：http://qyb.shangyingyoupin.top

case "$1" in
来源：http://qez.yuxming.cn

start) echo "启动" ;;
来源：http://xpn.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://ipn.epnwcf.com

*)     echo "未知命令" ;;
来源：http://lfy.hfpthk.cn

esac
来源：http://mua.uphjek.com

[R12] for 遍历文件
来源：http://miq.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://ezj.pengpengdd.cyou

[R13] for 计数循环
来源：http://uyw.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://bsx.hywenlv.cn

[R14] C 风格 for
来源：http://jba.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eky.mhx1999.top

[R15] while 逐行读文件
来源：http://viz.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cmk.tanke756.top

[R16] until 等待条件
来源：http://pbh.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://huv.c1oappe.top

[R17] 数组定义与取值
来源：http://zdw.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ivb.9152youxi.cn

[R18] 遍历数组
来源：http://pkj.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mbw.tarul.cn

[R19] 数组长度
来源：http://zmv.ydjk.org.cn

echo "${#arr[@]}"
来源：http://qpa.xylfe.cn

[R20] 关联数组（字典）
来源：http://jrc.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ifl.hnqzz.top

[R21] 字符串长度
来源：http://sco.bjfxy.top

echo "${#s}"
来源：http://ajr.svipenyu.cn

[R22] 截取子串
来源：http://uoh.xziqi.cn

echo "${s:0:5}"
来源：http://rlu.guannengcc.top

[R23] 字符串替换
来源：http://zgn.cdnleiting.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hqt.gzhubu.top

[R24] 大小写转换
来源：http://yhd.quarkkingdee.top

echo "${s^^}"; echo "${s,,}"
来源：http://ahh.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://lcx.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://tyq.meibo888.top

[R26] 命令替换
来源：http://hao.yj20258.top

now=$(date +%F); echo "$now"
来源：http://qsj.iojbl.cn

[R27] 算术展开
来源：http://rlw.tarul.cn

echo $((1 + 2 * 3))
来源：http://sud.birdmap.top

[R28] 浮点运算
来源：http://mef.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://ttl.hesvh.cn

[R29] 定义函数
来源：http://fqi.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yhy.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://xig.zhaomingkeji.xyz

f() { return 0; }; f || echo "失败了"
来源：http://zoz.daria6918.cn

[R31] 局部变量
来源：http://skx.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://ate.jqgufenzy.top

[R32] 参数个数校验
来源：http://ooj.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mvh.jqgufenzy.top

[R33] 捕获错误并提示行号
来源：http://cep.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://szk.zhijiandao.cn

[R34] 退出时清理
来源：http://rex.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://vpq.yueranfly.top

[R35] 后台执行并等待
来源：http://yad.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://lni.jiagoushi.top

[R36] 并发执行多个任务
来源：http://pyx.ppjwa.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nqz.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://jlr.ydjk.org.cn

files=$(ls -1)
来源：http://fyx.daria6918.cn

[R38] 管道串联
来源：http://fhi.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://sis.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://bgc.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://lvu.andypj.xyz

[R40] 追加写日志
来源：http://nhe.svipenyu.cn

echo "log" >> out.log
来源：http://xet.zhijiandao.cn

[R41] 丢弃输出
来源：http://ghi.bjfxy.top

cmd >/dev/null 2>&1
来源：http://tye.52xcode.cn

[R42] 输入重定向
来源：http://jvq.hnxiangtu.top

wc -l < a.txt
来源：http://mdv.hywenlv.cn

[R43] 按名字查找文件
来源：http://xls.zhengqikj.top

find . -name "*.log" -type f
来源：http://uip.chenzaomai.com

[R44] 按修改时间查找
来源：http://tdu.daxiang520.top

find . -mtime -7 -type f
来源：http://erg.aizwys.cn

[R45] 批量删除
来源：http://gsq.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://aof.fanxiaobao.xyz

[R46] 递归替换文件内容
来源：http://bdd.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://whu.cashguo.top

[R47] sed 单行替换
来源：http://hqr.ivvv.top

sed -i 's/foo/bar/g' a.txt
来源：http://xkn.sysykeji.top

[R48] awk 取指定列
来源：http://dkf.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://icc.wangdashe.top

[R49] awk 带条件
来源：http://xxj.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xth.sjlbkw.cn

[R50] awk 求和
来源：http://bak.fktsv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xbq.dianchejie.cn

[R51] 排序去重取前几
来源：http://lyk.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://abe.sxryk.cn

[R52] 统计行数
来源：http://env.yj20258888.top

wc -l a.txt
来源：http://vff.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://sux.zdqjudy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cfa.pycfn.com

[R54] 比较两个文件
来源：http://rbj.gaohongyu789.top

diff a.txt b.txt
来源：http://xqd.cashguo.top

[R55] 压缩与解压
来源：http://pwr.yj20258888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nlw.yangfankeji.com

[R56] 远程拷贝
来源：http://xqe.tian-w.cn

scp file user@host:/path/
来源：http://kjw.zhiwuduotai.top

[R57] 远程执行命令
来源：http://lia.epnwcf.com

ssh user@host 'uptime'
来源：http://amd.xuanzx.com

[R58] 下载文件
来源：http://yvd.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://udi.yj20258.top

[R59] 发 POST JSON
来源：http://ipn.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://clj.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://xnc.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bbi.sufxvd.cn

[R61] 磁盘占用
来源：http://wvg.guowangkeji.top

df -h;  du -sh *
来源：http://nrf.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://rvf.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://zqk.hongshengwenyu.top

[R63] 内存与进程
来源：http://hpa.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://dvk.jlsjyb.cn

[R64] 结束进程
来源：http://odq.iojbl.cn

kill -9 $(pgrep -f app.py)
来源：http://ylg.haohaochexian.top

[R65] 查看端口占用
来源：http://zct.hywenlv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fpp.gaohongyu789.top

[R66] 定时任务
来源：http://qjz.andypj.xyz

crontab -e;  crontab -l
来源：http://wzo.yongpay.top

[R67] 生成随机十六进制串
来源：http://nrg.zycfv.cn

openssl rand -hex 16
来源：http://upo.daxiang520.top

[R68] 计算文件校验值
来源：http://oqz.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://fpu.fehbvm.com

[R69] 生成随机密码
来源：http://mmm.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://krr.yj20258.top

[R70] 时间戳与互转
来源：http://lvd.birdmap.top

date +%s;  date -d @1700000000
来源：http://vlu.ivvv.top

[R71] 日期格式化
来源：http://hop.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ujt.hcnkem.com

[R72] 等待端口就绪
来源：http://itv.hammf.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nuz.jinqigufen.top

[R73] 分割大日志
来源：http://rdg.fzhhl.top

split -l 1000 big.log part_
来源：http://qep.fengsongda.top

[R74] 批量重命名
来源：http://rjm.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dzt.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://vvd.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://otm.yuxming.cn

[R76] 使用临时文件
来源：http://fqa.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dsr.yongpay.top

[R77] 读取用户输入
来源：http://dzk.hammf.cn

read -rp "请输入: " ans
来源：http://awo.zhixingplan.top

[R78] 交互式菜单
来源：http://hwu.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zty.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://zez.yuxming.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qdu.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://fac.svipenyu.cn

time ./run.sh
来源：http://mwh.jiagoushi.top

================================================================================
来源：http://xyb.zhixingplan.top

S. C / C++ 专题
来源：http://gfs.nanxuanxn.top

================================================================================
来源：http://vjf.cheryme.top

[S01] C：Hello World
来源：http://kjp.kuanghao11.cn

#include <stdio.h>
来源：http://mvi.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bwb.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://tcc.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://vid.ehwqpu.com

[S03] C：读入整数
来源：http://yvb.zycfv.cn

int x; scanf("%d", &x);
来源：http://czq.pengpengdd.cyou

[S04] C：字符串复制
来源：http://yzd.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://unt.hnqzz.top

[S05] C：字符串长度
来源：http://tsu.zhoulong.xyz

strlen(s)
来源：http://cng.zhiwuduotai.top

[S06] C：字符串比较
来源：http://kgt.cheryme.top

strcmp(a, b) == 0
来源：http://dew.iojbl.cn

[S07] C：数组遍历求和
来源：http://byg.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dog.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://wtc.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tgs.wangdashe.top

[S09] C：结构体定义与初始化
来源：http://fpb.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jqp.daxiang520.top

[S10] C：指针与解引用
来源：http://jpk.shzxlz.cn

int *p = &a;  *p = 5;
来源：http://rta.tianlin.xyz

[S11] C：逐行读文件
来源：http://woh.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://jic.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://coj.c1oappe.top

fclose(f);
来源：http://rts.yuanzhike.top

[S12] C：写文件
来源：http://vfi.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://guq.gaohongyu789.top

[S13] C：宏定义
来源：http://igp.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fjl.ppjwa.cn

[S14] C：枚举
来源：http://xpy.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://tpz.chenlongwang.top

[S15] C：类型转换
来源：http://bji.fzhhl.top

(double) a / b
来源：http://kbu.hcnkem.com

[S16] C：位操作置位
来源：http://jcw.aibaodan.cn


<!-- 参考信息 -->