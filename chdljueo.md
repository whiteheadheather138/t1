代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://qcb.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eas.smart0.xyz

[Q47] 与平均值比较
来源：http://jay.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hmo.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://nxa.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wxd.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://kkg.meibo888.top

[Q49] 更新单行
来源：http://ior.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ihj.jqgfzy.top

[Q50] 批量更新
来源：http://vyi.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mxx.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://izr.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ths.fengsongda.top

[Q52] 删除指定行
来源：http://czg.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://mxm.ehwqpu.com

[Q53] 按条件删除
来源：http://gig.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iks.pengpengdd.cyou

[Q54] 清空表
来源：http://yfj.birdmap.top

TRUNCATE TABLE logs;
来源：http://gso.hongshengwenyu.top

[Q55] 排名（并列占位）
来源：http://znq.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qit.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://iup.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ddp.sysykeji.top

[Q57] 行号
来源：http://whp.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bsq.fanxiaobao.xyz

[Q58] 累计求和
来源：http://php.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://suo.cucudq.cn

[Q59] 分组内累计
来源：http://yvb.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wan.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://szt.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qbb.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ypa.jqgufenzy.top

[Q61] 移动平均
来源：http://tqt.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mld.zhiwuduotai.top

[Q62] 分组占比
来源：http://shc.jlsjyb.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dlq.xylfe.cn

[Q63] 开启事务
来源：http://mpp.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fnq.svipenyu.cn

[Q64] 提交事务
来源：http://hag.tianlin.xyz

COMMIT;
来源：http://viq.andypj.xyz

[Q65] 回滚事务
来源：http://sez.yongpay.top

ROLLBACK;
来源：http://wlx.ppjwa.cn

[Q66] 行锁查询
来源：http://zkz.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bnw.yueranfly.top

[Q67] 设置隔离级别
来源：http://omi.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rvo.mhx1999.top

[Q68] 保存点
来源：http://fly.jinqigfzy.top

SAVEPOINT sp1;
来源：http://ctr.cashguo.top

ROLLBACK TO sp1;
来源：http://suc.yj20258.top

[Q69] 查看执行计划
来源：http://lyj.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xys.guowangkeji.top

[Q70] 更新统计信息
来源：http://vkx.cashguo.top

ANALYZE TABLE users;
来源：http://cyn.chenzaomai.com

[Q71] 查看建表语句
来源：http://bsv.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zhl.sjlbkw.cn

[Q72] 查看索引
来源：http://pub.yj20258.top

SHOW INDEX FROM users;
来源：http://aqp.chenjidiqi.icu

[Q73] 查看表状态
来源：http://laz.kuanghao11.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ijp.fengsongda.top

[Q74] 强制使用索引
来源：http://gcg.jyoumei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lyt.tarul.cn

[Q75] 日期格式化
来源：http://wty.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gwh.nanxinkj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zuq.uphjek.com

[Q76] 按天统计
来源：http://lgc.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zoh.aizwys.cn

[Q77] 时间加减
来源：http://pbh.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ihq.sjlbkw.cn

[Q78] 当前时间
来源：http://bbk.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gqg.aizwys.cn

[Q79] 字符串拼接
来源：http://evd.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ain.dashuyun.cn

[Q80] 字符串截取
来源：http://gnb.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mhs.0kj1m.cn

[Q81] 字符串替换
来源：http://wle.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qgk.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://mzr.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qsm.xylfe.cn

[Q83] 大小写转换
来源：http://xpo.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://amv.hammf.cn

[Q84] 去除首尾空格
来源：http://uec.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://jzd.jiagoushi.top

[Q85] 数值取整
来源：http://dvi.chenzaomai.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fia.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://jjt.hesvh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://luc.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://jgr.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lbj.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://uaw.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xrr.zhijiandao.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lce.dashuyun.cn

[Q89] 判断表是否存在
来源：http://lct.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bfn.hnxiangtu.top

[Q90] 生成序号列
来源：http://rql.ybcxt.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://shq.hesvh.cn

================================================================================
来源：http://mlo.pengpengdd.cyou

R. Bash 专题
来源：http://wvd.yj202588.top

================================================================================
来源：http://zli.jqgfzy.top

[R01] shebang 与严格模式
来源：http://cnj.hongshengwenyu.top

#!/usr/bin/env bash
来源：http://dtm.fktsv.cn

set -euo pipefail
来源：http://klp.pycfn.com

[R02] 变量赋值与使用
来源：http://yzn.zhixingplan.top

name="Tom"; echo "$name"
来源：http://ozw.tanke756.top

[R03] 只读变量
来源：http://elc.kuanghao11.cn

readonly PI=3.14
来源：http://fwe.bbcook.cn

[R04] 位置参数
来源：http://mcf.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jzy.snrcjt.cn

[R05] 参数默认值
来源：http://osk.pengpengdd.cyou

name="${1:-default}"
来源：http://lay.nanxinkj.top

[R06] 判断命令是否存在
来源：http://zsz.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xei.9152youxi.cn

[R07] if 判断文件
来源：http://rbx.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qrx.gaohongyu789.top

[R08] 数值比较
来源：http://dii.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tkc.yonumen.top

[R09] 字符串比较
来源：http://hpe.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bzx.cashguo.top

[R10] 正则匹配
来源：http://xdu.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dww.pycfn.com

[R11] case 多分支
来源：http://bsc.dianchejie.cn

case "$1" in
来源：http://pku.yfazqb.com

start) echo "启动" ;;
来源：http://vxz.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://car.yueranfly.top

*)     echo "未知命令" ;;
来源：http://wyg.fanxiaobao.xyz

esac
来源：http://eit.xuanzx.com

[R12] for 遍历文件
来源：http://bhb.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://dje.aizwys.cn

[R13] for 计数循环
来源：http://nif.316326.xyz

for i in {1..10}; do echo "$i"; done
来源：http://agw.yj20258888.top

[R14] C 风格 for
来源：http://rtm.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rle.haohaochexian.top

[R15] while 逐行读文件
来源：http://qkv.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dyy.cqqwz.cn

[R16] until 等待条件
来源：http://gkt.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dzw.cdnleiting.top

[R17] 数组定义与取值
来源：http://bgj.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://hii.sufxvd.cn

[R18] 遍历数组
来源：http://pxb.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qui.feifeiyinyue.top

[R19] 数组长度
来源：http://buk.bjfxy.top

echo "${#arr[@]}"
来源：http://jhw.gotoacloud.top

[R20] 关联数组（字典）
来源：http://sjt.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qne.ydzc1.top

[R21] 字符串长度
来源：http://icc.aizwys.cn

echo "${#s}"
来源：http://vgr.feifeiyinyue.top

[R22] 截取子串
来源：http://xej.ydzc1.top

echo "${s:0:5}"
来源：http://ozq.nwbrower.top

[R23] 字符串替换
来源：http://zyo.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vmu.jqgufenzy.top

[R24] 大小写转换
来源：http://gux.yangfankeji.com

echo "${s^^}"; echo "${s,,}"
来源：http://gpr.yongpay.top

[R25] 去后缀 / 去前缀
来源：http://rtf.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://unt.svipenyu.cn

[R26] 命令替换
来源：http://yqe.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://yjl.jyoumei.cn

[R27] 算术展开
来源：http://qrf.yj20258.top

echo $((1 + 2 * 3))
来源：http://sxm.shzxlz.cn

[R28] 浮点运算
来源：http://qvc.yonumen.top

echo "scale=2; 10/3" | bc
来源：http://mud.kuanghao11.cn

[R29] 定义函数
来源：http://ydd.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://raa.fehbvm.com

[R30] 函数返回状态码
来源：http://qzy.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://spu.ivvv.top

[R31] 局部变量
来源：http://amd.hfpthk.cn

f() { local x=1; echo "$x"; }
来源：http://cyn.dashuyun.cn

[R32] 参数个数校验
来源：http://gmu.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bgb.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://bbf.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gfh.yanxiufei.cn

[R34] 退出时清理
来源：http://dpw.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bfp.zhongyouzk.top

[R35] 后台执行并等待
来源：http://kzu.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://plf.vehdjk.com

[R36] 并发执行多个任务
来源：http://rrs.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jvf.xziqi.cn

[R37] 把输出赋给变量
来源：http://urz.epnwcf.com

files=$(ls -1)
来源：http://nuc.xziqi.cn

[R38] 管道串联
来源：http://jch.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://tlk.yj202588.top

[R39] 重定向标准输出与错误
来源：http://eqs.xinyue.icu

cmd > out.log 2>&1
来源：http://xdn.ybcxt.top

[R40] 追加写日志
来源：http://zea.hcnkem.com

echo "log" >> out.log
来源：http://ynl.xingfuxueyuan.xyz

[R41] 丢弃输出
来源：http://cyd.yangfankeji.com

cmd >/dev/null 2>&1
来源：http://upz.gotoacloud.top

[R42] 输入重定向
来源：http://wwh.mhx1999.top

wc -l < a.txt
来源：http://jlg.zdqjudy.top

[R43] 按名字查找文件
来源：http://pzg.sweek.top

find . -name "*.log" -type f
来源：http://hid.epnwcf.com

[R44] 按修改时间查找
来源：http://nob.shzxlz.cn

find . -mtime -7 -type f
来源：http://ere.yangfankeji.com

[R45] 批量删除
来源：http://tou.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://ohj.xinyue.icu

[R46] 递归替换文件内容
来源：http://huq.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://okj.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://ttx.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://raz.yongpay.top

[R48] awk 取指定列
来源：http://zqg.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://mow.hesvh.cn

[R49] awk 带条件
来源：http://rfu.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kfe.nanxuanxn.top

[R50] awk 求和
来源：http://zls.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fca.hfpthk.cn

[R51] 排序去重取前几
来源：http://rwo.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://blp.sjlbkw.cn

[R52] 统计行数
来源：http://oit.jlsjyb.cn

wc -l a.txt
来源：http://fms.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://lwz.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xdd.ydjk.org.cn

[R54] 比较两个文件
来源：http://aqw.yj202588.top

diff a.txt b.txt
来源：http://ksr.tanke756.top

[R55] 压缩与解压
来源：http://xjc.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lix.jinqigufen.top

[R56] 远程拷贝
来源：http://lbo.meibo888.top

scp file user@host:/path/
来源：http://wqd.andypj.xyz

[R57] 远程执行命令
来源：http://pnk.andypj.xyz

ssh user@host 'uptime'
来源：http://lpt.yvedp.cn

[R58] 下载文件
来源：http://sls.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nam.smart0.xyz

[R59] 发 POST JSON
来源：http://csv.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://swp.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://kwd.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mov.gogol.net.cn

[R61] 磁盘占用
来源：http://wwr.aibaodan.cn

df -h;  du -sh *
来源：http://alw.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://apv.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://xrj.ydzc1.top

[R63] 内存与进程
来源：http://eai.cashguo.top

free -h;  ps aux | grep nginx
来源：http://uok.52xcode.cn

[R64] 结束进程
来源：http://glr.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://yoa.yfazqb.com

[R65] 查看端口占用
来源：http://vzd.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rkx.jqgfzy.top

[R66] 定时任务
来源：http://coa.cheryme.top

crontab -e;  crontab -l
来源：http://riu.jinyuanbaomall.cn

[R67] 生成随机十六进制串
来源：http://xks.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://wrw.cashguo.top

[R68] 计算文件校验值
来源：http://qej.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://anw.sufxvd.cn

[R69] 生成随机密码
来源：http://aqf.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://jio.uphjek.com

[R70] 时间戳与互转
来源：http://snc.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://arq.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://dfs.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://edj.zhoulong.xyz

[R72] 等待端口就绪
来源：http://mkq.chenjidiqi.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://eti.yanxiufei.cn

[R73] 分割大日志
来源：http://pgq.guowangkeji.top

split -l 1000 big.log part_
来源：http://wcu.tanke756.top

[R74] 批量重命名
来源：http://kvi.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://brt.daxiang520.top

[R75] 导出环境变量
来源：http://bgz.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://sjz.jinqigfzy.top

[R76] 使用临时文件
来源：http://kch.yuanzhike.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://szi.ydjk.org.cn

[R77] 读取用户输入
来源：http://lea.zhongyouzk.top

read -rp "请输入: " ans
来源：http://zky.yanxiufei.cn

[R78] 交互式菜单
来源：http://lbv.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://oeb.xuanzx.com

[R79] 解析命令行选项
来源：http://pzu.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://llx.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://kub.dashuyun.cn

time ./run.sh
来源：http://sfx.jqgfzy.top

================================================================================
来源：http://ukp.hesvh.cn

S. C / C++ 专题
来源：http://gds.jqgufenzy.top

================================================================================
来源：http://lvg.vqdsnc.cn

[S01] C：Hello World
来源：http://kqp.wangdashe.top

#include <stdio.h>
来源：http://jou.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kqd.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://rog.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://xeu.fktsv.cn

[S03] C：读入整数
来源：http://vuw.hesvh.cn

int x; scanf("%d", &x);
来源：http://tja.cdnleiting.top

[S04] C：字符串复制
来源：http://xuv.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://vqe.uphjek.com

[S05] C：字符串长度
来源：http://sgv.cdnleiting.top

strlen(s)
来源：http://axm.fktsv.cn

[S06] C：字符串比较
来源：http://dec.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://kdu.xuanzx.com

[S07] C：数组遍历求和
来源：http://amf.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://exf.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://ypz.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xfl.yj20258.top

[S09] C：结构体定义与初始化
来源：http://bdx.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jsv.svipenyu.cn

[S10] C：指针与解引用
来源：http://afi.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://ayf.shuidangran.top

[S11] C：逐行读文件
来源：http://pta.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://kcq.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oeb.mhx1999.top

fclose(f);
来源：http://ekl.wangshuangyany.cn

[S12] C：写文件
来源：http://aba.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hpu.fktsv.cn

[S13] C：宏定义
来源：http://fcw.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eph.sufxvd.cn

[S14] C：枚举
来源：http://jsc.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://kyi.fengsongda.top

[S15] C：类型转换
来源：http://zcv.yonumen.top

(double) a / b
来源：http://pkv.hcnkem.com

[S16] C：位操作置位
来源：http://fha.fzhhl.top


<!-- 参考信息 -->