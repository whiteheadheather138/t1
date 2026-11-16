代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kne.yanxiufei.cn

[Q52] 删除指定行
来源：http://xch.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://xwf.tianlin.xyz

[Q53] 按条件删除
来源：http://zud.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kmp.nwbrower.top

[Q54] 清空表
来源：http://idx.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://eke.fzhhl.top

[Q55] 排名（并列占位）
来源：http://pqi.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://frh.yangfankeji.com

[Q56] 密集排名（并列不占位）
来源：http://fxp.yangfankeji.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uaq.quarkkingdee.top

[Q57] 行号
来源：http://efl.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ofc.chenlongwang.top

[Q58] 累计求和
来源：http://uxx.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ada.fehbvm.com

[Q59] 分组内累计
来源：http://mcn.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fqp.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://syw.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qlw.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://chr.shzxlz.cn

[Q61] 移动平均
来源：http://zqy.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fod.chenlongwang.top

[Q62] 分组占比
来源：http://qla.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mld.daria6918.cn

[Q63] 开启事务
来源：http://mzm.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eol.yj202588.top

[Q64] 提交事务
来源：http://flp.bbcook.cn

COMMIT;
来源：http://sbc.ivvv.top

[Q65] 回滚事务
来源：http://izx.svipenyu.cn

ROLLBACK;
来源：http://etn.vehdjk.com

[Q66] 行锁查询
来源：http://mcn.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sqr.daxiang520.top

[Q67] 设置隔离级别
来源：http://ltl.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gqg.jinyuanbaomall.cn

[Q68] 保存点
来源：http://rfa.ydzc1.top

SAVEPOINT sp1;
来源：http://hqy.wangdashe.top

ROLLBACK TO sp1;
来源：http://cvj.haohaochexian.top

[Q69] 查看执行计划
来源：http://tqj.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cqi.hywenlv.cn

[Q70] 更新统计信息
来源：http://mnu.cucudq.cn

ANALYZE TABLE users;
来源：http://qwx.gotoacloud.top

[Q71] 查看建表语句
来源：http://gve.hnxiangtu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://udb.bjfxy.top

[Q72] 查看索引
来源：http://diu.jianghu66.top

SHOW INDEX FROM users;
来源：http://yop.tianlin.xyz

[Q73] 查看表状态
来源：http://lza.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wle.yuanzhike.top

[Q74] 强制使用索引
来源：http://npv.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xaz.zdbjq.cn

[Q75] 日期格式化
来源：http://wql.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sdf.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ftw.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://wza.yj20258.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rcj.xuetiantiany.cn

[Q77] 时间加减
来源：http://jlx.bjfxy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bsz.tarul.cn

[Q78] 当前时间
来源：http://izy.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://avs.sjlbkw.cn

[Q79] 字符串拼接
来源：http://dyo.c1oappe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tkv.vehdjk.com

[Q80] 字符串截取
来源：http://qve.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nus.yuxming.cn

[Q81] 字符串替换
来源：http://cle.yvedp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xbd.ivvv.top

[Q82] 字符长度与字节长度
来源：http://jai.xuetiantiany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rye.snrcjt.cn

[Q83] 大小写转换
来源：http://ysu.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ldp.hfpthk.cn

[Q84] 去除首尾空格
来源：http://iow.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://hoq.zdbjq.cn

[Q85] 数值取整
来源：http://ryv.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xkm.yj202588.top

[Q86] 读取 JSON 字段
来源：http://cku.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://knm.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://bvs.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ywb.aizwys.cn

[Q88] 行转列（条件聚合）
来源：http://dru.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vfc.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wlf.jyoumei.cn

[Q89] 判断表是否存在
来源：http://gnb.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nwg.tanke756.top

[Q90] 生成序号列
来源：http://ogy.yonumen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vnt.zhixingplan.top

================================================================================
来源：http://kry.jqgufenzy.top

R. Bash 专题
来源：http://riq.jyoumei.cn

================================================================================
来源：http://gby.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://csv.ydjk.org.cn

#!/usr/bin/env bash
来源：http://zvb.wangdashe.top

set -euo pipefail
来源：http://ice.gogol.net.cn

[R02] 变量赋值与使用
来源：http://mpx.tianlin.xyz

name="Tom"; echo "$name"
来源：http://mbk.guannengcc.top

[R03] 只读变量
来源：http://oqw.fzhhl.top

readonly PI=3.14
来源：http://mge.guowangkeji.top

[R04] 位置参数
来源：http://jxm.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fmu.shanyushiyangtech.top

[R05] 参数默认值
来源：http://wja.tarul.cn

name="${1:-default}"
来源：http://nme.cqqwz.cn

[R06] 判断命令是否存在
来源：http://yrm.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://asc.jqgfzy.top

[R07] if 判断文件
来源：http://zgg.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aeb.hnxiangtu.top

[R08] 数值比较
来源：http://tsk.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fwp.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://zoa.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nfm.vehdjk.com

[R10] 正则匹配
来源：http://gyj.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mpj.nwbrower.top

[R11] case 多分支
来源：http://coc.cashguo.top

case "$1" in
来源：http://msf.pycfn.com

start) echo "启动" ;;
来源：http://udi.yueranfly.top

stop)  echo "停止" ;;
来源：http://cyp.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://imh.meibo888.top

esac
来源：http://wyl.zhijiandao.cn

[R12] for 遍历文件
来源：http://dib.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://dgz.yvedp.cn

[R13] for 计数循环
来源：http://xev.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://mke.zycfv.cn

[R14] C 风格 for
来源：http://gms.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kqf.jiagoushi.top

[R15] while 逐行读文件
来源：http://ryr.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://waf.jyoumei.cn

[R16] until 等待条件
来源：http://krh.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cuu.nwbrower.top

[R17] 数组定义与取值
来源：http://hge.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://kta.shzxlz.cn

[R18] 遍历数组
来源：http://aji.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mxf.yvedp.cn

[R19] 数组长度
来源：http://riw.ppjwa.cn

echo "${#arr[@]}"
来源：http://kvw.hongshengwenyu.top

[R20] 关联数组（字典）
来源：http://kkm.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kox.nanxuanxn.top

[R21] 字符串长度
来源：http://xfk.zhoulong.xyz

echo "${#s}"
来源：http://lqy.haohaochexian.top

[R22] 截取子串
来源：http://wxd.chenzaomai.com

echo "${s:0:5}"
来源：http://jde.sysykeji.top

[R23] 字符串替换
来源：http://ujf.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ymd.yj202588.top

[R24] 大小写转换
来源：http://zhv.shuidangran.top

echo "${s^^}"; echo "${s,,}"
来源：http://oca.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://sxu.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ntc.jqgfzy.top

[R26] 命令替换
来源：http://agz.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://mmc.zhongyouzk.top

[R27] 算术展开
来源：http://sxs.havefunace.top

echo $((1 + 2 * 3))
来源：http://xlk.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://tsy.xinyue.icu

echo "scale=2; 10/3" | bc
来源：http://jbx.jyoumei.cn

[R29] 定义函数
来源：http://nfb.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uxq.aizwys.cn

[R30] 函数返回状态码
来源：http://aoz.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://xfb.shanyushiyangtech.top

[R31] 局部变量
来源：http://mqp.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://rmz.pycfn.com

[R32] 参数个数校验
来源：http://wgq.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zcs.fktsv.cn

[R33] 捕获错误并提示行号
来源：http://wne.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wwr.redwolf501.top

[R34] 退出时清理
来源：http://biv.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://ned.jyoumei.cn

[R35] 后台执行并等待
来源：http://eyi.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gbd.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://fdr.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zbr.bjfxy.top

[R37] 把输出赋给变量
来源：http://qzb.fengsongda.top

files=$(ls -1)
来源：http://lmm.iojbl.cn

[R38] 管道串联
来源：http://xle.dianchejie.cn

cat a.txt | grep -i error | wc -l
来源：http://ekw.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://qns.yonumen.top

cmd > out.log 2>&1
来源：http://uxh.316326.xyz

[R40] 追加写日志
来源：http://onx.guannengcc.top

echo "log" >> out.log
来源：http://npq.snrcjt.cn

[R41] 丢弃输出
来源：http://kjq.fktsv.cn

cmd >/dev/null 2>&1
来源：http://dti.iojbl.cn

[R42] 输入重定向
来源：http://fwe.yonumen.top

wc -l < a.txt
来源：http://xtm.pycfn.com

[R43] 按名字查找文件
来源：http://svg.ivvv.top

find . -name "*.log" -type f
来源：http://ldk.ydjk.org.cn

[R44] 按修改时间查找
来源：http://gck.svipenyu.cn

find . -mtime -7 -type f
来源：http://dda.gogol.net.cn

[R45] 批量删除
来源：http://eyc.aizwys.cn

find . -name "*.tmp" -delete
来源：http://ujn.chenzaomai.com

[R46] 递归替换文件内容
来源：http://onf.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bhh.shzxlz.cn

[R47] sed 单行替换
来源：http://hpr.shangyingyoupin.top

sed -i 's/foo/bar/g' a.txt
来源：http://jdw.hcnkem.com

[R48] awk 取指定列
来源：http://kgy.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://xpn.redwolf501.top

[R49] awk 带条件
来源：http://xcw.dianchejie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eiv.jqgfzy.top

[R50] awk 求和
来源：http://poz.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yic.hysaishi.cn

[R51] 排序去重取前几
来源：http://ilq.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vts.sweek.top

[R52] 统计行数
来源：http://lhc.ydjk.org.cn

wc -l a.txt
来源：http://qbh.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://ceu.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ors.cashguo.top

[R54] 比较两个文件
来源：http://qhy.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://qqx.bjfxy.top

[R55] 压缩与解压
来源：http://jta.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ipz.aibaodan.cn

[R56] 远程拷贝
来源：http://bot.xinyue.icu

scp file user@host:/path/
来源：http://bxg.hongshengwenyu.top

[R57] 远程执行命令
来源：http://und.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://har.zycfv.cn

[R58] 下载文件
来源：http://khf.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pfq.vehdjk.com

[R59] 发 POST JSON
来源：http://jua.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://crs.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://ccl.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yji.guannengcc.top

[R61] 磁盘占用
来源：http://fii.xuanzx.com

df -h;  du -sh *
来源：http://neg.jqgfzy.top

[R62] 找最占空间的文件
来源：http://fbf.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://dgn.mhx1999.top

[R63] 内存与进程
来源：http://zxg.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://xxv.nwbrower.top

[R64] 结束进程
来源：http://vlm.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://ipv.quarkkingdee.top

[R65] 查看端口占用
来源：http://xvn.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mob.shzxlz.cn

[R66] 定时任务
来源：http://lcp.cashguo.top

crontab -e;  crontab -l
来源：http://csu.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://tzg.wangdashe.top

openssl rand -hex 16
来源：http://bfv.chenzaomai.com

[R68] 计算文件校验值
来源：http://usc.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rxt.chenjidiqi.icu

[R69] 生成随机密码
来源：http://nfr.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://tlf.sjlbkw.cn

[R70] 时间戳与互转
来源：http://hth.yuxming.cn

date +%s;  date -d @1700000000
来源：http://pwv.jyoumei.cn

[R71] 日期格式化
来源：http://pwk.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pkn.hfpthk.cn

[R72] 等待端口就绪
来源：http://gew.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jxr.hywenlv.cn

[R73] 分割大日志
来源：http://ukx.fktsv.cn

split -l 1000 big.log part_
来源：http://ord.nanxuanxn.top

[R74] 批量重命名
来源：http://qsr.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yrk.fktsv.cn

[R75] 导出环境变量
来源：http://ybi.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://knz.vehdjk.com

[R76] 使用临时文件
来源：http://nzz.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zhb.jianghu66.top

[R77] 读取用户输入
来源：http://god.jlsjyb.cn

read -rp "请输入: " ans
来源：http://stz.iojbl.cn

[R78] 交互式菜单
来源：http://yzp.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://grx.gaohongyu789.top

[R79] 解析命令行选项
来源：http://ijk.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yuq.uphjek.com

[R80] 查看脚本执行耗时
来源：http://mev.ydzc1.top

time ./run.sh
来源：http://qvl.jinqigfzy.top

================================================================================
来源：http://tbv.zhongyouzk.top

S. C / C++ 专题
来源：http://aux.mhx1999.top

================================================================================
来源：http://zir.shuidangran.top

[S01] C：Hello World
来源：http://cle.guowangkeji.top

#include <stdio.h>
来源：http://tnq.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://usu.sysykeji.top

[S02] C：变量与格式化输出
来源：http://ikz.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://san.316326.xyz

[S03] C：读入整数
来源：http://lnc.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://uof.52xcode.cn

[S04] C：字符串复制
来源：http://cnv.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qym.cqqwz.cn

[S05] C：字符串长度
来源：http://wrx.fzhhl.top

strlen(s)
来源：http://pok.hcnkem.com

[S06] C：字符串比较
来源：http://dne.xziqi.cn

strcmp(a, b) == 0
来源：http://ovg.sysykeji.top

[S07] C：数组遍历求和
来源：http://hji.guowangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fhi.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://mgb.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://enh.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://xuw.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pih.tian-w.cn

[S10] C：指针与解引用
来源：http://ekf.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://opr.zhoulong.xyz

[S11] C：逐行读文件
来源：http://ttz.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://ahn.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bcc.fzhhl.top

fclose(f);
来源：http://oom.jianghu66.top

[S12] C：写文件
来源：http://llq.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://elp.hywenlv.cn

[S13] C：宏定义
来源：http://fio.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hpu.epnwcf.com

[S14] C：枚举
来源：http://exj.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://wdu.hammf.cn

[S15] C：类型转换
来源：http://ymk.0kj1m.cn

(double) a / b
来源：http://ssf.sxryk.cn

[S16] C：位操作置位
来源：http://qgb.mhx1999.top

x |= (1 << 3);
来源：http://euq.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://naj.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yig.chenlongwang.top

[S18] C：命令行参数
来源：http://ctp.fktsv.cn

int main(int argc, char **argv)
来源：http://cyx.yuanzhike.top

[S19] C：快速排序
来源：http://exc.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://qhc.kuanghao11.cn

[S20] C：二分查找
来源：http://kbn.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hoq.hammf.cn

[S21] C：字符类别判断
来源：http://jjx.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ica.chenzaomai.com

[S22] C：字符串转数字
来源：http://zab.cheryme.top


<!-- 参考信息 -->