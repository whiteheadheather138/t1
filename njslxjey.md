代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qpv.shanyushiyangtech.top

[Q52] 删除指定行
来源：http://nye.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://qmg.uphjek.com

[Q53] 按条件删除
来源：http://pvj.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dbm.tarul.cn

[Q54] 清空表
来源：http://swz.chenzaomai.com

TRUNCATE TABLE logs;
来源：http://zmq.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://ksy.jqgufenzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://czd.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://xog.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bts.zhixingplan.top

[Q57] 行号
来源：http://ezp.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://psq.andypj.xyz

[Q58] 累计求和
来源：http://lsy.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sbe.hammf.cn

[Q59] 分组内累计
来源：http://wtw.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vis.fzhhl.top

[Q60] 取上一行 / 下一行
来源：http://tgn.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kfy.ehwqpu.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kxn.nanxuanxn.top

[Q61] 移动平均
来源：http://hco.sjlbkw.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kbw.jqgfzy.top

[Q62] 分组占比
来源：http://nqt.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://otx.gzhubu.top

[Q63] 开启事务
来源：http://nvk.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ptz.haohaochexian.top

[Q64] 提交事务
来源：http://irn.meibo888.top

COMMIT;
来源：http://evi.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://kpq.snrcjt.cn

ROLLBACK;
来源：http://zfo.daxiang520.top

[Q66] 行锁查询
来源：http://nsu.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zyl.xuanzx.com

[Q67] 设置隔离级别
来源：http://qkv.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qtx.shanyushiyangkeji.top

[Q68] 保存点
来源：http://nuj.dashuyun.cn

SAVEPOINT sp1;
来源：http://anw.ehwqpu.com

ROLLBACK TO sp1;
来源：http://edn.dianchejie.cn

[Q69] 查看执行计划
来源：http://qxm.yonumen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gcb.jyoumei.cn

[Q70] 更新统计信息
来源：http://gjn.cashguo.top

ANALYZE TABLE users;
来源：http://kqj.wangdashe.top

[Q71] 查看建表语句
来源：http://rbi.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qfr.redwolf501.top

[Q72] 查看索引
来源：http://fws.yuanzhike.top

SHOW INDEX FROM users;
来源：http://hnk.wangshuangyany.cn

[Q73] 查看表状态
来源：http://jan.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gzo.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://luz.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://myw.cashguo.top

[Q75] 日期格式化
来源：http://vxa.ydzc1.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ziq.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ozj.xylfe.cn

[Q76] 按天统计
来源：http://wbs.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xnp.jianghu66.top

[Q77] 时间加减
来源：http://qfo.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eua.epnwcf.com

[Q78] 当前时间
来源：http://izb.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nst.hesvh.cn

[Q79] 字符串拼接
来源：http://ywj.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hdw.jiagoushi.top

[Q80] 字符串截取
来源：http://otg.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jrx.jyoumei.cn

[Q81] 字符串替换
来源：http://wcn.tarul.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hcf.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://kmn.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oic.fktsv.cn

[Q83] 大小写转换
来源：http://wjf.xylfe.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pkp.jyoumei.cn

[Q84] 去除首尾空格
来源：http://say.chenzaomai.com

SELECT TRIM(name) FROM users;
来源：http://kzk.sufxvd.cn

[Q85] 数值取整
来源：http://oqc.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tar.hnxiangtu.top

[Q86] 读取 JSON 字段
来源：http://aqs.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pgd.yj202588.top

[Q87] JSON 字段做条件
来源：http://whp.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nbu.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://ltc.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qes.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lbc.zycfv.cn

[Q89] 判断表是否存在
来源：http://ovf.hysaishi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dtr.zdqjudy.top

[Q90] 生成序号列
来源：http://djm.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mks.0kj1m.cn

================================================================================
来源：http://ffk.smart0.xyz

R. Bash 专题
来源：http://jgd.smart0.xyz

================================================================================
来源：http://wto.smart0.xyz

[R01] shebang 与严格模式
来源：http://kmo.tianlin.xyz

#!/usr/bin/env bash
来源：http://ghq.cheryme.top

set -euo pipefail
来源：http://roy.yuxming.cn

[R02] 变量赋值与使用
来源：http://oeo.316326.xyz

name="Tom"; echo "$name"
来源：http://nng.fengsongda.top

[R03] 只读变量
来源：http://cgv.xuetiantiany.cn

readonly PI=3.14
来源：http://uqm.hongshengwenyu.top

[R04] 位置参数
来源：http://cpl.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qgg.nwbrower.top

[R05] 参数默认值
来源：http://mrq.yvedp.cn

name="${1:-default}"
来源：http://qji.xylfe.cn

[R06] 判断命令是否存在
来源：http://qdv.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ymu.vehdjk.com

[R07] if 判断文件
来源：http://lgw.chenzaomai.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aps.jiagoushi.top

[R08] 数值比较
来源：http://fzu.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tdi.hnqzz.top

[R09] 字符串比较
来源：http://tpc.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dsm.shanyushiyangtech.top

[R10] 正则匹配
来源：http://dib.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cuq.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://knf.zhongyouzk.top

case "$1" in
来源：http://mlp.ivvv.top

start) echo "启动" ;;
来源：http://exw.shanyushiyangtech.top

stop)  echo "停止" ;;
来源：http://mzr.gzhubu.top

*)     echo "未知命令" ;;
来源：http://xck.smart0.xyz

esac
来源：http://yhw.0kj1m.cn

[R12] for 遍历文件
来源：http://bcg.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://ojf.haohaochexian.top

[R13] for 计数循环
来源：http://vje.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://xwg.zhoulong.xyz

[R14] C 风格 for
来源：http://qik.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wgb.9152youxi.cn

[R15] while 逐行读文件
来源：http://faa.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uoc.snrcjt.cn

[R16] until 等待条件
来源：http://qjy.pycfn.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tmz.cucudq.cn

[R17] 数组定义与取值
来源：http://zwf.pengpengdd.cyou

arr=(a b c); echo "${arr[0]}"
来源：http://xwt.fktsv.cn

[R18] 遍历数组
来源：http://mjy.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wrt.cdnleiting.top

[R19] 数组长度
来源：http://uek.jianghu66.top

echo "${#arr[@]}"
来源：http://smn.ppjwa.cn

[R20] 关联数组（字典）
来源：http://ryy.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pmx.fengsongda.top

[R21] 字符串长度
来源：http://byw.9152youxi.cn

echo "${#s}"
来源：http://len.aizwys.cn

[R22] 截取子串
来源：http://azj.tianlin.xyz

echo "${s:0:5}"
来源：http://wor.ivvv.top

[R23] 字符串替换
来源：http://ojq.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lku.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://rmp.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://gmv.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://aem.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rfs.nanxuanxn.top

[R26] 命令替换
来源：http://dah.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://cwk.zycfv.cn

[R27] 算术展开
来源：http://rrb.cucudq.cn

echo $((1 + 2 * 3))
来源：http://vyj.kuanghao11.cn

[R28] 浮点运算
来源：http://scc.yj20258.top

echo "scale=2; 10/3" | bc
来源：http://ogd.fzhhl.top

[R29] 定义函数
来源：http://sru.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cjh.aizwys.cn

[R30] 函数返回状态码
来源：http://evp.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://gcz.aibaodan.cn

[R31] 局部变量
来源：http://rxt.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://sta.cdnleiting.top

[R32] 参数个数校验
来源：http://tsj.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pda.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://jzb.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xkk.jianghu66.top

[R34] 退出时清理
来源：http://hhp.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://sth.sweek.top

[R35] 后台执行并等待
来源：http://oos.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://wfh.yj202588.top

[R36] 并发执行多个任务
来源：http://znb.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xro.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://ndl.ivvv.top

files=$(ls -1)
来源：http://ojj.redwolf501.top

[R38] 管道串联
来源：http://uuw.fengsongda.top

cat a.txt | grep -i error | wc -l
来源：http://mnv.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://fln.yvedp.cn

cmd > out.log 2>&1
来源：http://qfm.tianlin.xyz

[R40] 追加写日志
来源：http://irf.ybcxt.top

echo "log" >> out.log
来源：http://itl.cdnleiting.top

[R41] 丢弃输出
来源：http://yop.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://fcq.chenlongwang.top

[R42] 输入重定向
来源：http://tnq.jqgufenzy.top

wc -l < a.txt
来源：http://ijb.yfazqb.com

[R43] 按名字查找文件
来源：http://dlk.xziqi.cn

find . -name "*.log" -type f
来源：http://eyx.cdnleiting.top

[R44] 按修改时间查找
来源：http://itr.yj202588.top

find . -mtime -7 -type f
来源：http://yju.wangdashe.top

[R45] 批量删除
来源：http://lrj.tanke756.top

find . -name "*.tmp" -delete
来源：http://psk.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://ink.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://udh.aibaodan.cn

[R47] sed 单行替换
来源：http://apm.cucudq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wlk.shzxlz.cn

[R48] awk 取指定列
来源：http://qya.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://wvx.epnwcf.com

[R49] awk 带条件
来源：http://www.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://olz.daria6918.cn

[R50] awk 求和
来源：http://ryw.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fdz.jinqigfzy.top

[R51] 排序去重取前几
来源：http://fhx.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://jmo.xuanzx.com

[R52] 统计行数
来源：http://enf.zhongyouzk.top

wc -l a.txt
来源：http://afl.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://pke.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dre.jyoumei.cn

[R54] 比较两个文件
来源：http://iwg.hywenlv.cn

diff a.txt b.txt
来源：http://sxu.zycfv.cn

[R55] 压缩与解压
来源：http://cxm.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lec.jqgfzy.top

[R56] 远程拷贝
来源：http://nps.snrcjt.cn

scp file user@host:/path/
来源：http://onm.9152youxi.cn

[R57] 远程执行命令
来源：http://dyu.52xcode.cn

ssh user@host 'uptime'
来源：http://szd.sweek.top

[R58] 下载文件
来源：http://lon.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eyo.hnqzz.top

[R59] 发 POST JSON
来源：http://fpk.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vzu.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://qoy.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ucl.jinqigufen.top

[R61] 磁盘占用
来源：http://vqe.fanxiaobao.xyz

df -h;  du -sh *
来源：http://xce.haohaochexian.top

[R62] 找最占空间的文件
来源：http://dht.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://usl.yueranfly.top

[R63] 内存与进程
来源：http://rfe.tian-w.cn

free -h;  ps aux | grep nginx
来源：http://xbd.ybcxt.top

[R64] 结束进程
来源：http://bbp.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://rpt.ydjk.org.cn

[R65] 查看端口占用
来源：http://cty.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://seu.fktsv.cn

[R66] 定时任务
来源：http://wgp.gogol.net.cn

crontab -e;  crontab -l
来源：http://etk.nanxinkj.top

[R67] 生成随机十六进制串
来源：http://bwk.hammf.cn

openssl rand -hex 16
来源：http://htc.sweek.top

[R68] 计算文件校验值
来源：http://qak.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aaj.ydjk.org.cn

[R69] 生成随机密码
来源：http://oxw.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://vle.ydzc1.top

[R70] 时间戳与互转
来源：http://jds.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://vxo.uphjek.com

[R71] 日期格式化
来源：http://vuw.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tod.quarkkingdee.top

[R72] 等待端口就绪
来源：http://sxj.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pcj.zhijiandao.cn

[R73] 分割大日志
来源：http://ogb.guannengcc.top

split -l 1000 big.log part_
来源：http://wrt.gzhubu.top

[R74] 批量重命名
来源：http://cjx.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dgp.ydjk.org.cn

[R75] 导出环境变量
来源：http://zdy.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://bfz.hnqzz.top

[R76] 使用临时文件
来源：http://hjz.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jzb.xylfe.cn

[R77] 读取用户输入
来源：http://yzk.zhixingplan.top

read -rp "请输入: " ans
来源：http://ziz.yj20258888.top

[R78] 交互式菜单
来源：http://hxw.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sjf.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://say.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://res.cheryme.top

[R80] 查看脚本执行耗时
来源：http://afp.havefunace.top

time ./run.sh
来源：http://zzd.zhengqikj.top

================================================================================
来源：http://vbq.dashuyun.cn

S. C / C++ 专题
来源：http://khl.smart0.xyz

================================================================================
来源：http://jcd.vqdsnc.cn

[S01] C：Hello World
来源：http://sru.tarul.cn

#include <stdio.h>
来源：http://mtq.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://brx.gzhubu.top

[S02] C：变量与格式化输出
来源：http://byb.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://olb.hcnkem.com

[S03] C：读入整数
来源：http://ycj.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://axg.ydzc1.top

[S04] C：字符串复制
来源：http://pzb.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://mcf.zdbjq.cn

[S05] C：字符串长度
来源：http://hhh.ywan-chungtsiang.top

strlen(s)
来源：http://nvu.sxryk.cn

[S06] C：字符串比较
来源：http://fvv.xziqi.cn

strcmp(a, b) == 0
来源：http://vjk.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://uop.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dqj.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://ple.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sqx.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://mkd.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hlf.xylfe.cn

[S10] C：指针与解引用
来源：http://okw.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://mts.sweek.top

[S11] C：逐行读文件
来源：http://pbz.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://ios.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pqf.yj20258.top

fclose(f);
来源：http://fjq.jinqigfzy.top

[S12] C：写文件
来源：http://xbx.jiagoushi.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yek.9152youxi.cn

[S13] C：宏定义
来源：http://jjl.jianghu66.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qgk.fzhhl.top

[S14] C：枚举
来源：http://zxn.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://lqd.jianghu66.top

[S15] C：类型转换
来源：http://dem.gogol.net.cn

(double) a / b
来源：http://tex.yuanzhike.top

[S16] C：位操作置位
来源：http://hrt.vehdjk.com

x |= (1 << 3);
来源：http://yns.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://wum.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ndf.haohaochexian.top

[S18] C：命令行参数
来源：http://nch.bjfxy.top

int main(int argc, char **argv)
来源：http://ltr.cqqwz.cn

[S19] C：快速排序
来源：http://cih.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jtz.vehdjk.com

[S20] C：二分查找
来源：http://sso.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tif.smart0.xyz

[S21] C：字符类别判断
来源：http://ivp.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rtk.aibaodan.cn

[S22] C：字符串转数字
来源：http://udq.dianchejie.cn


<!-- 参考信息 -->