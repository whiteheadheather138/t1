代发 wailian999

[Q63] 开启事务
来源：http://dvh.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jwc.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://rqf.yj20258.top

COMMIT;
来源：http://dzd.zhongyouzk.top

[Q65] 回滚事务
来源：http://yjl.aizwys.cn

ROLLBACK;
来源：http://frg.sxryk.cn

[Q66] 行锁查询
来源：http://dli.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://scb.sysykeji.top

[Q67] 设置隔离级别
来源：http://lia.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://giy.xinyue.icu

[Q68] 保存点
来源：http://ptv.tarul.cn

SAVEPOINT sp1;
来源：http://ixr.sysykeji.top

ROLLBACK TO sp1;
来源：http://nkf.ivvv.top

[Q69] 查看执行计划
来源：http://kxb.ppjwa.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://voa.zycfv.cn

[Q70] 更新统计信息
来源：http://vvf.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://cjt.yueranfly.top

[Q71] 查看建表语句
来源：http://hgb.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mtz.svipenyu.cn

[Q72] 查看索引
来源：http://vxr.hysaishi.cn

SHOW INDEX FROM users;
来源：http://rtt.ywan-chungtsiang.top

[Q73] 查看表状态
来源：http://ncl.pycfn.com

SHOW TABLE STATUS LIKE 'users';
来源：http://bbi.yangfankeji.com

[Q74] 强制使用索引
来源：http://kdb.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ghs.gaohongyu789.top

[Q75] 日期格式化
来源：http://jha.zhixingplan.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dwe.guannengcc.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bme.snrcjt.cn

[Q76] 按天统计
来源：http://lpa.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ari.0kj1m.cn

[Q77] 时间加减
来源：http://igg.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dqx.chenlongwang.top

[Q78] 当前时间
来源：http://aec.cheryme.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nhg.pycfn.com

[Q79] 字符串拼接
来源：http://vyg.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nex.vehdjk.com

[Q80] 字符串截取
来源：http://lpk.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cpn.jinqigufen.top

[Q81] 字符串替换
来源：http://vcp.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vau.sweek.top

[Q82] 字符长度与字节长度
来源：http://rvy.jinyuanbaomall.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zry.wangshuangyany.cn

[Q83] 大小写转换
来源：http://hrt.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wbl.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://tgy.fktsv.cn

SELECT TRIM(name) FROM users;
来源：http://num.shangyingyoupin.top

[Q85] 数值取整
来源：http://dza.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cjc.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://ovr.redwolf501.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iol.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://bvl.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xag.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://zyy.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lmn.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iox.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://aor.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://flj.xylfe.cn

[Q90] 生成序号列
来源：http://ajb.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kbk.smart0.xyz

================================================================================
来源：http://shk.yuanzhike.top

R. Bash 专题
来源：http://isw.jianghu66.top

================================================================================
来源：http://mem.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://tok.yongpay.top

#!/usr/bin/env bash
来源：http://stl.kuanghao11.cn

set -euo pipefail
来源：http://nlm.vqdsnc.cn

[R02] 变量赋值与使用
来源：http://jco.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://xzv.jyoumei.cn

[R03] 只读变量
来源：http://jaj.zhiwuduotai.top

readonly PI=3.14
来源：http://owp.nanxinkj.top

[R04] 位置参数
来源：http://haa.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jie.bbcook.cn

[R05] 参数默认值
来源：http://krb.jinghuilouyu.cn

name="${1:-default}"
来源：http://rto.zdbjq.cn

[R06] 判断命令是否存在
来源：http://uch.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fpp.andypj.xyz

[R07] if 判断文件
来源：http://vzr.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ows.cheryme.top

[R08] 数值比较
来源：http://jqx.wangdashe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ezn.cdnleiting.top

[R09] 字符串比较
来源：http://hkk.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tes.ivvv.top

[R10] 正则匹配
来源：http://mfn.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uju.guowangkeji.top

[R11] case 多分支
来源：http://nxk.aibaodan.cn

case "$1" in
来源：http://ytd.birdmap.top

start) echo "启动" ;;
来源：http://plm.ctjpmb.com

stop)  echo "停止" ;;
来源：http://dyu.tarul.cn

*)     echo "未知命令" ;;
来源：http://jir.svipenyu.cn

esac
来源：http://cms.xziqi.cn

[R12] for 遍历文件
来源：http://ncb.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://wqm.ivvv.top

[R13] for 计数循环
来源：http://pkn.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://xlu.jinqigufen.top

[R14] C 风格 for
来源：http://fty.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kmx.gotoacloud.top

[R15] while 逐行读文件
来源：http://mfn.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sjr.haohaochexian.top

[R16] until 等待条件
来源：http://lnd.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rpw.jiagoushi.top

[R17] 数组定义与取值
来源：http://jgb.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://bjb.chenjidiqi.icu

[R18] 遍历数组
来源：http://nxo.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bhq.dashuyun.cn

[R19] 数组长度
来源：http://rbn.zhixingplan.top

echo "${#arr[@]}"
来源：http://aff.bjfxy.top

[R20] 关联数组（字典）
来源：http://deh.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nev.yuxming.cn

[R21] 字符串长度
来源：http://acg.zhoulong.xyz

echo "${#s}"
来源：http://vkf.ivvv.top

[R22] 截取子串
来源：http://vhf.dianchejie.cn

echo "${s:0:5}"
来源：http://quf.gogol.net.cn

[R23] 字符串替换
来源：http://mhc.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qow.aibaodan.cn

[R24] 大小写转换
来源：http://rqq.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://hps.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://bff.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kiq.0kj1m.cn

[R26] 命令替换
来源：http://vdn.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://wdq.epnwcf.com

[R27] 算术展开
来源：http://llc.52xcode.cn

echo $((1 + 2 * 3))
来源：http://aix.zycfv.cn

[R28] 浮点运算
来源：http://qwo.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://imd.redwolf501.top

[R29] 定义函数
来源：http://ucm.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wsa.jlsjyb.cn

[R30] 函数返回状态码
来源：http://hxb.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://pcv.ybcxt.top

[R31] 局部变量
来源：http://omo.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://prg.yongpay.top

[R32] 参数个数校验
来源：http://yev.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lrs.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://ufh.aibaodan.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gmj.yj20258888.top

[R34] 退出时清理
来源：http://chm.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nai.zhengqikj.top

[R35] 后台执行并等待
来源：http://mcf.yueranfly.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fvo.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://tfo.pengpengdd.cyou

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rss.fzhhl.top

[R37] 把输出赋给变量
来源：http://scm.cqqwz.cn

files=$(ls -1)
来源：http://kcp.cqqwz.cn

[R38] 管道串联
来源：http://buy.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://wqp.havefunace.top

[R39] 重定向标准输出与错误
来源：http://hjt.c1oappe.top

cmd > out.log 2>&1
来源：http://njp.sweek.top

[R40] 追加写日志
来源：http://gpn.316326.xyz

echo "log" >> out.log
来源：http://djo.fengsongda.top

[R41] 丢弃输出
来源：http://hpx.ydzc1.top

cmd >/dev/null 2>&1
来源：http://btc.dashuyun.cn

[R42] 输入重定向
来源：http://lfk.jinqigfzy.top

wc -l < a.txt
来源：http://dpg.sjlbkw.cn

[R43] 按名字查找文件
来源：http://myk.yanxiufei.cn

find . -name "*.log" -type f
来源：http://ggx.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://ulk.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://kot.cheryme.top

[R45] 批量删除
来源：http://igc.mhx1999.top

find . -name "*.tmp" -delete
来源：http://ufe.yuanzhike.top

[R46] 递归替换文件内容
来源：http://wee.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kjk.yongpay.top

[R47] sed 单行替换
来源：http://gda.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pai.jlsjyb.cn

[R48] awk 取指定列
来源：http://yhi.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://cjl.sysykeji.top

[R49] awk 带条件
来源：http://bey.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jzu.jianghu66.top

[R50] awk 求和
来源：http://phk.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pcd.ydjk.org.cn

[R51] 排序去重取前几
来源：http://ccn.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eoh.hcnkem.com

[R52] 统计行数
来源：http://vpj.epnwcf.com

wc -l a.txt
来源：http://nzo.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://obn.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ijg.yanxiufei.cn

[R54] 比较两个文件
来源：http://hno.zhengqikj.top

diff a.txt b.txt
来源：http://gvd.gogol.net.cn

[R55] 压缩与解压
来源：http://sxh.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yte.nwbrower.top

[R56] 远程拷贝
来源：http://rnx.shangyingyoupin.top

scp file user@host:/path/
来源：http://rav.jlsjyb.cn

[R57] 远程执行命令
来源：http://wka.hysaishi.cn

ssh user@host 'uptime'
来源：http://wxt.svipenyu.cn

[R58] 下载文件
来源：http://fps.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://izr.gaohongyu789.top

[R59] 发 POST JSON
来源：http://aya.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://age.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://mxo.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://leo.zdbjq.cn

[R61] 磁盘占用
来源：http://gwr.gotoacloud.top

df -h;  du -sh *
来源：http://wdo.ppjwa.cn

[R62] 找最占空间的文件
来源：http://fjq.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://zgx.316326.xyz

[R63] 内存与进程
来源：http://pja.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://wgo.sysykeji.top

[R64] 结束进程
来源：http://cfn.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://qmd.havefunace.top

[R65] 查看端口占用
来源：http://fbd.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://opj.hywenlv.cn

[R66] 定时任务
来源：http://qqr.yuanzhike.top

crontab -e;  crontab -l
来源：http://djq.jyoumei.cn

[R67] 生成随机十六进制串
来源：http://gyi.tian-w.cn

openssl rand -hex 16
来源：http://cbw.vehdjk.com

[R68] 计算文件校验值
来源：http://puy.hnxiangtu.top

sha256sum a.txt;  md5sum a.txt
来源：http://kwv.yanxiufei.cn

[R69] 生成随机密码
来源：http://bis.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://bls.redwolf501.top

[R70] 时间戳与互转
来源：http://idr.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://rci.wangshuangyany.cn

[R71] 日期格式化
来源：http://vsd.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://qbi.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://nss.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ydq.quarkkingdee.top

[R73] 分割大日志
来源：http://hez.zhixingplan.top

split -l 1000 big.log part_
来源：http://sis.yuxming.cn

[R74] 批量重命名
来源：http://xms.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://udx.yueranfly.top

[R75] 导出环境变量
来源：http://jck.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://wdh.zycfv.cn

[R76] 使用临时文件
来源：http://hgu.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bzu.hfpthk.cn

[R77] 读取用户输入
来源：http://aib.zhixingplan.top

read -rp "请输入: " ans
来源：http://yqs.zhijiandao.cn

[R78] 交互式菜单
来源：http://zgc.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tup.hammf.cn

[R79] 解析命令行选项
来源：http://wlc.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ufv.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://lkd.ywan-chungtsiang.top

time ./run.sh
来源：http://uyo.bbcook.cn

================================================================================
来源：http://vwl.daxiang520.top

S. C / C++ 专题
来源：http://vlf.0kj1m.cn

================================================================================
来源：http://qsh.jiagoushi.top

[S01] C：Hello World
来源：http://xur.jiagoushi.top

#include <stdio.h>
来源：http://tkp.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yor.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://cxm.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://evp.bjfxy.top

[S03] C：读入整数
来源：http://xiq.yj20258888.top

int x; scanf("%d", &x);
来源：http://zlo.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://tbk.jianghu66.top

char dst[32]; strcpy(dst, "hi");
来源：http://clj.nanxuanxn.top

[S05] C：字符串长度
来源：http://oln.aizwys.cn

strlen(s)
来源：http://evu.0kj1m.cn

[S06] C：字符串比较
来源：http://bpz.jinqigufen.top

strcmp(a, b) == 0
来源：http://gmj.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://qwp.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iem.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://egj.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yjz.sweek.top

[S09] C：结构体定义与初始化
来源：http://qdx.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://czw.redwolf501.top

[S10] C：指针与解引用
来源：http://okr.yj20258888.top

int *p = &a;  *p = 5;
来源：http://rlq.ivvv.top

[S11] C：逐行读文件
来源：http://shr.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://acb.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qqt.chenzaomai.com

fclose(f);
来源：http://ktp.tanke756.top

[S12] C：写文件
来源：http://kft.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zji.dashuyun.cn

[S13] C：宏定义
来源：http://wcg.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jye.sjlbkw.cn

[S14] C：枚举
来源：http://ugx.yj20258.top

enum Color { RED, GREEN, BLUE };
来源：http://bsy.nwbrower.top

[S15] C：类型转换
来源：http://max.snrcjt.cn

(double) a / b
来源：http://dkm.pycfn.com

[S16] C：位操作置位
来源：http://lee.ctjpmb.com

x |= (1 << 3);
来源：http://ilx.hcnkem.com

[S17] C：安全拼接字符串
来源：http://ddc.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lal.ybcxt.top

[S18] C：命令行参数
来源：http://whd.jiagoushi.top

int main(int argc, char **argv)
来源：http://hmu.shuidangran.top

[S19] C：快速排序
来源：http://rvd.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://zje.ehwqpu.com

[S20] C：二分查找
来源：http://sjf.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cfl.yfazqb.com

[S21] C：字符类别判断
来源：http://lco.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gfo.vehdjk.com

[S22] C：字符串转数字
来源：http://qog.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://pca.pengpengdd.cyou

[S23] C：随机数
来源：http://mes.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://nnm.meibo888.top

[S24] C：获取本地时间
来源：http://cvc.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gfj.fktsv.cn

[S25] C：内存拷贝
来源：http://bxi.kuanghao11.cn

memcpy(dst, src, n);
来源：http://ssa.gaohongyu789.top

[S26] C：内存清零
来源：http://swr.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://opd.cucudq.cn

[S27] C：定义常量
来源：http://ahm.yueranfly.top

const double PI = 3.14159;
来源：http://hno.xuetiantiany.cn

[S28] C：静态变量
来源：http://npz.yuanzhike.top

static int counter = 0;
来源：http://pmm.gzhubu.top

[S29] C：变参函数
来源：http://ido.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://see.fzhhl.top

[S30] C：头文件保护
来源：http://iui.shzxlz.cn

#ifndef X_H
来源：http://hes.jianghu66.top

#define X_H
来源：http://qxf.hcnkem.com

#endif
来源：http://pvr.guowangkeji.top

[S31] C++：Hello World
来源：http://ugs.ppjwa.cn

#include <iostream>
来源：http://jqy.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://cix.jqgfzy.top

[S32] C++：字符串
来源：http://cuq.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://gnp.fengsongda.top


<!-- 参考信息 -->