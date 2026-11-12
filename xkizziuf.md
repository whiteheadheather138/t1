代发 wailian999

[Q48] CTE 公用表表达式
来源：http://xmw.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lcn.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://okm.shangyingyoupin.top

[Q49] 更新单行
来源：http://uqw.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iae.quarkkingdee.top

[Q50] 批量更新
来源：http://xva.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jmn.hysaishi.cn

[Q51] 用子查询更新
来源：http://tuv.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xqz.zhengqikj.top

[Q52] 删除指定行
来源：http://jhz.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://bzq.52xcode.cn

[Q53] 按条件删除
来源：http://bex.snrcjt.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://siq.zhijiandao.cn

[Q54] 清空表
来源：http://mxu.hfpthk.cn

TRUNCATE TABLE logs;
来源：http://pfo.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://lxd.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zrf.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://xfw.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sty.snrcjt.cn

[Q57] 行号
来源：http://psw.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cha.hywenlv.cn

[Q58] 累计求和
来源：http://tke.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xzi.aibaodan.cn

[Q59] 分组内累计
来源：http://evm.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zvn.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://ufb.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zis.aibaodan.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wqe.9152youxi.cn

[Q61] 移动平均
来源：http://wsa.havefunace.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jhr.yonumen.top

[Q62] 分组占比
来源：http://nqs.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dql.guannengcc.top

[Q63] 开启事务
来源：http://obt.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tjk.c1oappe.top

[Q64] 提交事务
来源：http://wva.dianchejie.cn

COMMIT;
来源：http://vbb.yuanzhike.top

[Q65] 回滚事务
来源：http://mud.yuanzhike.top

ROLLBACK;
来源：http://fly.ctjpmb.com

[Q66] 行锁查询
来源：http://hic.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://krf.c1oappe.top

[Q67] 设置隔离级别
来源：http://yxi.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yxc.hcnkem.com

[Q68] 保存点
来源：http://bzh.jinqigfzy.top

SAVEPOINT sp1;
来源：http://kno.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://zul.sufxvd.cn

[Q69] 查看执行计划
来源：http://wrr.chenjidiqi.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vem.yuanzhike.top

[Q70] 更新统计信息
来源：http://kmf.nanxinkj.top

ANALYZE TABLE users;
来源：http://tbb.c1oappe.top

[Q71] 查看建表语句
来源：http://blr.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nwm.zhaomingkeji.xyz

[Q72] 查看索引
来源：http://yss.ydzc1.top

SHOW INDEX FROM users;
来源：http://rdw.hammf.cn

[Q73] 查看表状态
来源：http://phc.tanke756.top

SHOW TABLE STATUS LIKE 'users';
来源：http://esf.shuidangran.top

[Q74] 强制使用索引
来源：http://rhw.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ufm.pengpengdd.cyou

[Q75] 日期格式化
来源：http://blv.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yfn.hysaishi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bhd.daria6918.cn

[Q76] 按天统计
来源：http://igm.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://paw.zhiwuduotai.top

[Q77] 时间加减
来源：http://ngj.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mqj.ivvv.top

[Q78] 当前时间
来源：http://lll.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hay.meibo888.top

[Q79] 字符串拼接
来源：http://acs.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bkd.zdqjudy.top

[Q80] 字符串截取
来源：http://wry.ybcxt.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://drg.yj20258.top

[Q81] 字符串替换
来源：http://sui.hcnkem.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://txx.yangfankeji.com

[Q82] 字符长度与字节长度
来源：http://rkb.zdbjq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lha.xinyue.icu

[Q83] 大小写转换
来源：http://drg.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://guv.jinqigufen.top

[Q84] 去除首尾空格
来源：http://bqm.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://rxj.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://esj.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://son.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://pzl.chenlongwang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ppz.52xcode.cn

[Q87] JSON 字段做条件
来源：http://gav.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tdm.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://cuq.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kxt.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zkt.svipenyu.cn

[Q89] 判断表是否存在
来源：http://vmx.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yhc.iojbl.cn

[Q90] 生成序号列
来源：http://ulx.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ufb.zdqjudy.top

================================================================================
来源：http://ikt.xylfe.cn

R. Bash 专题
来源：http://unj.tian-w.cn

================================================================================
来源：http://fbr.zhoulong.xyz

[R01] shebang 与严格模式
来源：http://fdn.sjlbkw.cn

#!/usr/bin/env bash
来源：http://ion.birdmap.top

set -euo pipefail
来源：http://imd.feifeiyinyue.top

[R02] 变量赋值与使用
来源：http://mvm.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://mml.wangdashe.top

[R03] 只读变量
来源：http://zjs.snrcjt.cn

readonly PI=3.14
来源：http://ubv.andypj.xyz

[R04] 位置参数
来源：http://hpa.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fwp.shuidangran.top

[R05] 参数默认值
来源：http://irx.jianghu66.top

name="${1:-default}"
来源：http://ili.gzhubu.top

[R06] 判断命令是否存在
来源：http://fad.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mpl.xuanzx.com

[R07] if 判断文件
来源：http://slj.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zay.xuetiantiany.cn

[R08] 数值比较
来源：http://xna.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dhy.chenlongwang.top

[R09] 字符串比较
来源：http://cxd.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bmx.gotoacloud.top

[R10] 正则匹配
来源：http://bca.shanyushiyangtech.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ash.yangfankeji.com

[R11] case 多分支
来源：http://kgo.zdbjq.cn

case "$1" in
来源：http://uzx.sufxvd.cn

start) echo "启动" ;;
来源：http://kfe.yonumen.top

stop)  echo "停止" ;;
来源：http://ded.yfazqb.com

*)     echo "未知命令" ;;
来源：http://ghu.9152youxi.cn

esac
来源：http://azd.daria6918.cn

[R12] for 遍历文件
来源：http://kiz.hnqzz.top

for f in *.txt; do echo "$f"; done
来源：http://zhh.yonumen.top

[R13] for 计数循环
来源：http://uze.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://ghk.xingfuxueyuan.xyz

[R14] C 风格 for
来源：http://zmi.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xug.hnxiangtu.top

[R15] while 逐行读文件
来源：http://ica.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://brc.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://igf.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://klz.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://jbj.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oqe.yj20258888.top

[R18] 遍历数组
来源：http://tec.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uwa.haohaochexian.top

[R19] 数组长度
来源：http://yvs.pycfn.com

echo "${#arr[@]}"
来源：http://uua.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://ych.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://snf.hywenlv.cn

[R21] 字符串长度
来源：http://qgp.chenzaomai.com

echo "${#s}"
来源：http://obv.redwolf501.top

[R22] 截取子串
来源：http://bnt.ctjpmb.com

echo "${s:0:5}"
来源：http://fzj.daria6918.cn

[R23] 字符串替换
来源：http://prt.yangfankeji.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://suz.hnqzz.top

[R24] 大小写转换
来源：http://rlg.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://ory.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://bdt.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lyp.zhongyouzk.top

[R26] 命令替换
来源：http://kje.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://mow.ywan-chungtsiang.top

[R27] 算术展开
来源：http://hta.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://bro.feifeiyinyue.top

[R28] 浮点运算
来源：http://yka.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://oca.hysaishi.cn

[R29] 定义函数
来源：http://myl.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xau.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://huh.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://tsf.hnqzz.top

[R31] 局部变量
来源：http://xdo.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://uhv.xylfe.cn

[R32] 参数个数校验
来源：http://lyw.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tzd.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://ulu.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://osl.hnxiangtu.top

[R34] 退出时清理
来源：http://lob.shanyushiyangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://uoh.yongpay.top

[R35] 后台执行并等待
来源：http://frl.birdmap.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ckl.hcnkem.com

[R36] 并发执行多个任务
来源：http://nvo.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ypa.chenlongwang.top

[R37] 把输出赋给变量
来源：http://pph.aibaodan.cn

files=$(ls -1)
来源：http://pcg.daxiang520.top

[R38] 管道串联
来源：http://lpf.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://qyv.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://bwk.hysaishi.cn

cmd > out.log 2>&1
来源：http://tdl.smart0.xyz

[R40] 追加写日志
来源：http://rcq.uphjek.com

echo "log" >> out.log
来源：http://xis.aibaodan.cn

[R41] 丢弃输出
来源：http://ole.52xcode.cn

cmd >/dev/null 2>&1
来源：http://ces.zhongyouzk.top

[R42] 输入重定向
来源：http://oqc.ehwqpu.com

wc -l < a.txt
来源：http://srx.9152youxi.cn

[R43] 按名字查找文件
来源：http://qgx.zhaomingkeji.xyz

find . -name "*.log" -type f
来源：http://czc.ehwqpu.com

[R44] 按修改时间查找
来源：http://xpb.ppjwa.cn

find . -mtime -7 -type f
来源：http://prd.tanke756.top

[R45] 批量删除
来源：http://mfb.bjfxy.top

find . -name "*.tmp" -delete
来源：http://qcb.52xcode.cn

[R46] 递归替换文件内容
来源：http://myy.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tey.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://qnz.yuanzhike.top

sed -i 's/foo/bar/g' a.txt
来源：http://ejb.yuxming.cn

[R48] awk 取指定列
来源：http://glm.nanxuanxn.top

awk '{print $1, $3}' a.txt
来源：http://mzx.zhixingplan.top

[R49] awk 带条件
来源：http://pvv.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tnx.yj202588.top

[R50] awk 求和
来源：http://wop.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cof.zhoulong.xyz

[R51] 排序去重取前几
来源：http://xpa.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qpb.zhaomingkeji.xyz

[R52] 统计行数
来源：http://gln.zdbjq.cn

wc -l a.txt
来源：http://qun.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://dbs.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mks.vehdjk.com

[R54] 比较两个文件
来源：http://mdi.uphjek.com

diff a.txt b.txt
来源：http://pxc.jinqigfzy.top

[R55] 压缩与解压
来源：http://oan.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://txl.yuxming.cn

[R56] 远程拷贝
来源：http://zay.kuanghao11.cn

scp file user@host:/path/
来源：http://arc.chenlongwang.top

[R57] 远程执行命令
来源：http://ltv.hnqzz.top

ssh user@host 'uptime'
来源：http://bse.yangfankeji.com

[R58] 下载文件
来源：http://vvn.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kug.zhixingplan.top

[R59] 发 POST JSON
来源：http://brh.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eqq.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://stx.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nzh.jqgufenzy.top

[R61] 磁盘占用
来源：http://ccl.yonumen.top

df -h;  du -sh *
来源：http://bit.yfazqb.com

[R62] 找最占空间的文件
来源：http://thk.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://ovy.zycfv.cn

[R63] 内存与进程
来源：http://qoj.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://wnk.0kj1m.cn

[R64] 结束进程
来源：http://trb.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://zbk.316326.xyz

[R65] 查看端口占用
来源：http://oak.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://peq.pycfn.com

[R66] 定时任务
来源：http://fzs.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://sem.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://bav.zhijiandao.cn

openssl rand -hex 16
来源：http://phw.zhixingplan.top

[R68] 计算文件校验值
来源：http://vro.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://mbw.feifeiyinyue.top

[R69] 生成随机密码
来源：http://zcz.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://ijz.xinyue.icu

[R70] 时间戳与互转
来源：http://kkc.ydzc1.top

date +%s;  date -d @1700000000
来源：http://gdo.meibo888.top

[R71] 日期格式化
来源：http://rdy.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fgd.zdbjq.cn

[R72] 等待端口就绪
来源：http://cnx.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://orb.jiagoushi.top

[R73] 分割大日志
来源：http://dmi.zhongyouzk.top

split -l 1000 big.log part_
来源：http://etc.feifeiyinyue.top

[R74] 批量重命名
来源：http://oik.uphjek.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fio.aizwys.cn

[R75] 导出环境变量
来源：http://pud.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://wny.svipenyu.cn

[R76] 使用临时文件
来源：http://wgg.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pzy.zhiwuduotai.top

[R77] 读取用户输入
来源：http://kir.hywenlv.cn

read -rp "请输入: " ans
来源：http://kty.hfpthk.cn

[R78] 交互式菜单
来源：http://ocp.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://axj.bjfxy.top

[R79] 解析命令行选项
来源：http://wby.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ksy.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://efw.bbcook.cn

time ./run.sh
来源：http://bkq.gaohongyu789.top

================================================================================
来源：http://rbs.yj202588.top

S. C / C++ 专题
来源：http://hqg.tian-w.cn

================================================================================
来源：http://lrt.zhiwuduotai.top

[S01] C：Hello World
来源：http://jax.sjlbkw.cn

#include <stdio.h>
来源：http://bam.hnqzz.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hul.aizwys.cn

[S02] C：变量与格式化输出
来源：http://mtd.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://xoq.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://seg.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://acx.9152youxi.cn

[S04] C：字符串复制
来源：http://wof.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://fat.shuidangran.top

[S05] C：字符串长度
来源：http://uzs.sysykeji.top

strlen(s)
来源：http://qrc.sxryk.cn

[S06] C：字符串比较
来源：http://uhn.9152youxi.cn

strcmp(a, b) == 0
来源：http://zti.tian-w.cn

[S07] C：数组遍历求和
来源：http://wot.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xkf.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://bkd.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wol.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://ear.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tnl.daria6918.cn

[S10] C：指针与解引用
来源：http://uzg.cashguo.top

int *p = &a;  *p = 5;
来源：http://fev.ehwqpu.com

[S11] C：逐行读文件
来源：http://ucg.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://tsq.dianchejie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nii.aizwys.cn

fclose(f);
来源：http://wua.nanxinkj.top

[S12] C：写文件
来源：http://gtu.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xva.cdnleiting.top

[S13] C：宏定义
来源：http://btu.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xtw.fanxiaobao.xyz

[S14] C：枚举
来源：http://yoj.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://pmo.meibo888.top

[S15] C：类型转换
来源：http://vql.gzhubu.top

(double) a / b
来源：http://drl.yonumen.top

[S16] C：位操作置位
来源：http://rnd.gzhubu.top

x |= (1 << 3);
来源：http://ifj.sxryk.cn

[S17] C：安全拼接字符串
来源：http://kxs.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hgd.cqqwz.cn

[S18] C：命令行参数
来源：http://uxj.jqgufenzy.top


<!-- 参考信息 -->