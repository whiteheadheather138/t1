代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nbh.hnxiangtu.top

[Q54] 清空表
来源：http://shp.gaohongyu789.top

TRUNCATE TABLE logs;
来源：http://evy.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://yhh.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aos.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://ypt.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ngc.jiagoushi.top

[Q57] 行号
来源：http://rzq.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nkw.fehbvm.com

[Q58] 累计求和
来源：http://fjf.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ekj.snrcjt.cn

[Q59] 分组内累计
来源：http://fva.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://okv.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://vch.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pbu.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://loz.cqqwz.cn

[Q61] 移动平均
来源：http://ydt.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vuu.ydzc1.top

[Q62] 分组占比
来源：http://bdt.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ndb.sufxvd.cn

[Q63] 开启事务
来源：http://ulo.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ayv.9152youxi.cn

[Q64] 提交事务
来源：http://qwd.ctjpmb.com

COMMIT;
来源：http://ibe.tian-w.cn

[Q65] 回滚事务
来源：http://uvi.yuxming.cn

ROLLBACK;
来源：http://npk.mhx1999.top

[Q66] 行锁查询
来源：http://oqr.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ghl.ybcxt.top

[Q67] 设置隔离级别
来源：http://hhh.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://omn.jqgufenzy.top

[Q68] 保存点
来源：http://puy.kuanghao11.cn

SAVEPOINT sp1;
来源：http://njj.ppjwa.cn

ROLLBACK TO sp1;
来源：http://rfk.316326.xyz

[Q69] 查看执行计划
来源：http://vst.jlsjyb.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ngn.yonumen.top

[Q70] 更新统计信息
来源：http://xuj.ehwqpu.com

ANALYZE TABLE users;
来源：http://mgj.zhongyouzk.top

[Q71] 查看建表语句
来源：http://fro.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pbe.tarul.cn

[Q72] 查看索引
来源：http://dfx.xuanzx.com

SHOW INDEX FROM users;
来源：http://bcs.shuidangran.top

[Q73] 查看表状态
来源：http://ixo.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://olc.dashuyun.cn

[Q74] 强制使用索引
来源：http://unv.fengsongda.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mkx.vehdjk.com

[Q75] 日期格式化
来源：http://koa.9152youxi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fbx.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uks.jinqigufen.top

[Q76] 按天统计
来源：http://qsh.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nyt.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://wtv.jyoumei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dhq.hysaishi.cn

[Q78] 当前时间
来源：http://acu.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ksw.chenzaomai.com

[Q79] 字符串拼接
来源：http://zwp.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gaf.zhiwuduotai.top

[Q80] 字符串截取
来源：http://hln.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ssq.gogol.net.cn

[Q81] 字符串替换
来源：http://erp.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xty.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://wfl.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cvv.jyoumei.cn

[Q83] 大小写转换
来源：http://tgg.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://osy.uphjek.com

[Q84] 去除首尾空格
来源：http://uqe.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://weq.bjfxy.top

[Q85] 数值取整
来源：http://vmz.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jux.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://ibp.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ezl.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://dpa.hysaishi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xar.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://sim.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://thc.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://duc.shangyingyoupin.top

[Q89] 判断表是否存在
来源：http://vxp.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jmb.daria6918.cn

[Q90] 生成序号列
来源：http://kbb.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zjp.yueranfly.top

================================================================================
来源：http://zfc.zdbjq.cn

R. Bash 专题
来源：http://tdq.xinyue.icu

================================================================================
来源：http://ndv.vehdjk.com

[R01] shebang 与严格模式
来源：http://gnf.cdnleiting.top

#!/usr/bin/env bash
来源：http://sbr.jinqigufen.top

set -euo pipefail
来源：http://mwi.wangdashe.top

[R02] 变量赋值与使用
来源：http://ecl.shuidangran.top

name="Tom"; echo "$name"
来源：http://gbj.xuetiantiany.cn

[R03] 只读变量
来源：http://xao.cucudq.cn

readonly PI=3.14
来源：http://ejj.sweek.top

[R04] 位置参数
来源：http://ofd.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mxt.zycfv.cn

[R05] 参数默认值
来源：http://bit.nanxuanxn.top

name="${1:-default}"
来源：http://aks.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://ibp.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uhe.tian-w.cn

[R07] if 判断文件
来源：http://wzw.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kjx.xuanzx.com

[R08] 数值比较
来源：http://nya.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ssd.zhijiandao.cn

[R09] 字符串比较
来源：http://zsh.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lxt.guannengcc.top

[R10] 正则匹配
来源：http://zlx.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zqx.fengsongda.top

[R11] case 多分支
来源：http://sby.quarkkingdee.top

case "$1" in
来源：http://qwl.jinqigufen.top

start) echo "启动" ;;
来源：http://cqm.uphjek.com

stop)  echo "停止" ;;
来源：http://msy.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://cmx.yonumen.top

esac
来源：http://axo.jqgfzy.top

[R12] for 遍历文件
来源：http://kuw.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://ryt.dianchejie.cn

[R13] for 计数循环
来源：http://aqr.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://qyr.yueranfly.top

[R14] C 风格 for
来源：http://uui.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://owz.mhx1999.top

[R15] while 逐行读文件
来源：http://isw.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://azy.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://emo.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://esu.shzxlz.cn

[R17] 数组定义与取值
来源：http://wbi.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://dvo.smart0.xyz

[R18] 遍历数组
来源：http://vuu.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://btq.tarul.cn

[R19] 数组长度
来源：http://rvz.zdbjq.cn

echo "${#arr[@]}"
来源：http://gsy.zdqjudy.top

[R20] 关联数组（字典）
来源：http://eya.havefunace.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lgb.shuidangran.top

[R21] 字符串长度
来源：http://iaj.jiagoushi.top

echo "${#s}"
来源：http://btr.yfazqb.com

[R22] 截取子串
来源：http://ibj.sweek.top

echo "${s:0:5}"
来源：http://uvv.chenzaomai.com

[R23] 字符串替换
来源：http://uqc.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eof.jinghuilouyu.cn

[R24] 大小写转换
来源：http://mvo.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://dyq.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://vzq.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://mjx.jinyuanbaomall.cn

[R26] 命令替换
来源：http://kkw.yj20258.top

now=$(date +%F); echo "$now"
来源：http://huh.0kj1m.cn

[R27] 算术展开
来源：http://xdp.yj20258.top

echo $((1 + 2 * 3))
来源：http://qqu.fktsv.cn

[R28] 浮点运算
来源：http://jwa.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://igi.shangyingyoupin.top

[R29] 定义函数
来源：http://cgn.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://erz.yfazqb.com

[R30] 函数返回状态码
来源：http://wnw.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://bot.aizwys.cn

[R31] 局部变量
来源：http://ino.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://acm.ppjwa.cn

[R32] 参数个数校验
来源：http://qof.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oru.ivvv.top

[R33] 捕获错误并提示行号
来源：http://kgi.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bym.fzhhl.top

[R34] 退出时清理
来源：http://zyr.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://apm.hesvh.cn

[R35] 后台执行并等待
来源：http://kqw.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pwh.yj20258888.top

[R36] 并发执行多个任务
来源：http://xgk.yj202588.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://chm.tianlin.xyz

[R37] 把输出赋给变量
来源：http://fsi.yanxiufei.cn

files=$(ls -1)
来源：http://pwz.cucudq.cn

[R38] 管道串联
来源：http://rrm.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://kys.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://lil.0kj1m.cn

cmd > out.log 2>&1
来源：http://ydt.daxiang520.top

[R40] 追加写日志
来源：http://ita.haohaochexian.top

echo "log" >> out.log
来源：http://ztc.jlsjyb.cn

[R41] 丢弃输出
来源：http://gxm.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://gjc.jqgfzy.top

[R42] 输入重定向
来源：http://hkj.dianchejie.cn

wc -l < a.txt
来源：http://qbc.guowangkeji.top

[R43] 按名字查找文件
来源：http://fyt.yuanzhike.top

find . -name "*.log" -type f
来源：http://xwa.jlsjyb.cn

[R44] 按修改时间查找
来源：http://ipo.ydzc1.top

find . -mtime -7 -type f
来源：http://fca.jqgfzy.top

[R45] 批量删除
来源：http://oli.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://krr.guowangkeji.top

[R46] 递归替换文件内容
来源：http://qcm.tian-w.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kvx.shzxlz.cn

[R47] sed 单行替换
来源：http://hlc.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://brx.uphjek.com

[R48] awk 取指定列
来源：http://fow.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://nij.gogol.net.cn

[R49] awk 带条件
来源：http://ovj.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rqg.tarul.cn

[R50] awk 求和
来源：http://isb.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://ovh.shuidangran.top

[R51] 排序去重取前几
来源：http://hwf.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://lvg.xuanzx.com

[R52] 统计行数
来源：http://nae.ehwqpu.com

wc -l a.txt
来源：http://cpd.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://ifi.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vla.quarkkingdee.top

[R54] 比较两个文件
来源：http://ywq.jyoumei.cn

diff a.txt b.txt
来源：http://laz.nanxuanxn.top

[R55] 压缩与解压
来源：http://avg.zhaomingkeji.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://efh.tanke756.top

[R56] 远程拷贝
来源：http://shh.fengsongda.top

scp file user@host:/path/
来源：http://htq.fzhhl.top

[R57] 远程执行命令
来源：http://ups.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://znz.yfazqb.com

[R58] 下载文件
来源：http://std.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vdy.shuidangran.top

[R59] 发 POST JSON
来源：http://crm.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://opc.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://myr.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lod.hongshengwenyu.top

[R61] 磁盘占用
来源：http://yth.tarul.cn

df -h;  du -sh *
来源：http://gct.yuanzhike.top

[R62] 找最占空间的文件
来源：http://csq.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://ewm.chenlongwang.top

[R63] 内存与进程
来源：http://zqc.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://krf.sysykeji.top

[R64] 结束进程
来源：http://fyo.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://euj.xylfe.cn

[R65] 查看端口占用
来源：http://gvh.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cpt.nwbrower.top

[R66] 定时任务
来源：http://ipn.jyoumei.cn

crontab -e;  crontab -l
来源：http://zbm.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://ozb.xziqi.cn

openssl rand -hex 16
来源：http://mgm.jinqigufen.top

[R68] 计算文件校验值
来源：http://ngc.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://fbn.jyoumei.cn

[R69] 生成随机密码
来源：http://idz.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://xie.dashuyun.cn

[R70] 时间戳与互转
来源：http://cun.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://fde.smart0.xyz

[R71] 日期格式化
来源：http://rjq.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://atw.hnqzz.top

[R72] 等待端口就绪
来源：http://hqp.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sis.tarul.cn

[R73] 分割大日志
来源：http://ryz.jiagoushi.top

split -l 1000 big.log part_
来源：http://qxe.vqdsnc.cn

[R74] 批量重命名
来源：http://gbk.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sjt.hcnkem.com

[R75] 导出环境变量
来源：http://fhm.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://jsg.zhiwuduotai.top

[R76] 使用临时文件
来源：http://yyg.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pfy.andypj.xyz

[R77] 读取用户输入
来源：http://plo.svipenyu.cn

read -rp "请输入: " ans
来源：http://qum.zycfv.cn

[R78] 交互式菜单
来源：http://dku.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bko.jqgfzy.top

[R79] 解析命令行选项
来源：http://hej.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kys.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://wlb.fanxiaobao.xyz

time ./run.sh
来源：http://htg.jianghu66.top

================================================================================
来源：http://vac.yfazqb.com

S. C / C++ 专题
来源：http://gni.sufxvd.cn

================================================================================
来源：http://soy.xziqi.cn

[S01] C：Hello World
来源：http://sto.yj20258.top

#include <stdio.h>
来源：http://bpn.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zut.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://vjo.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://til.sufxvd.cn

[S03] C：读入整数
来源：http://kxg.hcnkem.com

int x; scanf("%d", &x);
来源：http://ylq.ctjpmb.com

[S04] C：字符串复制
来源：http://zad.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uvw.uphjek.com

[S05] C：字符串长度
来源：http://oza.nanxuanxn.top

strlen(s)
来源：http://auc.pengpengdd.cyou

[S06] C：字符串比较
来源：http://vdx.gotoacloud.top

strcmp(a, b) == 0
来源：http://lip.cqqwz.cn

[S07] C：数组遍历求和
来源：http://qsm.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zad.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://zbj.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wgd.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://kbm.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hhx.dianchejie.cn

[S10] C：指针与解引用
来源：http://ult.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://pwf.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://qdf.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://isf.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ngn.xziqi.cn

fclose(f);
来源：http://iww.feifeiyinyue.top

[S12] C：写文件
来源：http://qmm.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://syq.ywan-chungtsiang.top

[S13] C：宏定义
来源：http://jlx.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kaz.yangfankeji.com

[S14] C：枚举
来源：http://upg.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://dpr.hysaishi.cn

[S15] C：类型转换
来源：http://aoz.aizwys.cn

(double) a / b
来源：http://jrd.nanxuanxn.top

[S16] C：位操作置位
来源：http://eqx.sysykeji.top

x |= (1 << 3);
来源：http://qjz.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://vxg.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://epm.c1oappe.top

[S18] C：命令行参数
来源：http://ocd.hfpthk.cn

int main(int argc, char **argv)
来源：http://azd.yueranfly.top

[S19] C：快速排序
来源：http://mpt.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mxl.shanyushiyangtech.top

[S20] C：二分查找
来源：http://yzq.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://krb.hfpthk.cn

[S21] C：字符类别判断
来源：http://oca.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cfd.pycfn.com

[S22] C：字符串转数字
来源：http://jyo.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sqa.shzxlz.cn

[S23] C：随机数
来源：http://xez.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ufj.zhongyouzk.top

[S24] C：获取本地时间
来源：http://agr.andypj.xyz


<!-- 参考信息 -->