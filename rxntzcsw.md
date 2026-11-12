代发 wailian999

[Q67] 设置隔离级别
来源：http://igm.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xum.feifeiyinyue.top

[Q68] 保存点
来源：http://dzx.tian-w.cn

SAVEPOINT sp1;
来源：http://hyd.zdqjudy.top

ROLLBACK TO sp1;
来源：http://psi.shanyushiyangkeji.top

[Q69] 查看执行计划
来源：http://zmf.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wsj.yuanzhike.top

[Q70] 更新统计信息
来源：http://omp.fktsv.cn

ANALYZE TABLE users;
来源：http://mlb.redwolf501.top

[Q71] 查看建表语句
来源：http://iur.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cug.pengpengdd.cyou

[Q72] 查看索引
来源：http://vdw.ivvv.top

SHOW INDEX FROM users;
来源：http://vzb.cashguo.top

[Q73] 查看表状态
来源：http://dfr.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://agy.ydjk.org.cn

[Q74] 强制使用索引
来源：http://rzf.gotoacloud.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wsj.xinyue.icu

[Q75] 日期格式化
来源：http://van.yuanzhike.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ibz.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jiy.redwolf501.top

[Q76] 按天统计
来源：http://dhh.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ekj.birdmap.top

[Q77] 时间加减
来源：http://oyr.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ojc.aizwys.cn

[Q78] 当前时间
来源：http://mod.fehbvm.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fgs.nanxinkj.top

[Q79] 字符串拼接
来源：http://sqx.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zxm.c1oappe.top

[Q80] 字符串截取
来源：http://gju.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iqq.hammf.cn

[Q81] 字符串替换
来源：http://pot.hongshengwenyu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nev.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://qdq.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://svf.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://jdy.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ccu.zycfv.cn

[Q84] 去除首尾空格
来源：http://jre.feifeiyinyue.top

SELECT TRIM(name) FROM users;
来源：http://tmt.feifeiyinyue.top

[Q85] 数值取整
来源：http://nmk.316326.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kvg.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://thc.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ppw.smart0.xyz

[Q87] JSON 字段做条件
来源：http://bse.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mdt.aizwys.cn

[Q88] 行转列（条件聚合）
来源：http://tgh.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nfg.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bfv.quarkkingdee.top

[Q89] 判断表是否存在
来源：http://gyc.shzxlz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sbn.yangfankeji.com

[Q90] 生成序号列
来源：http://szl.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iyd.yvedp.cn

================================================================================
来源：http://tvf.c1oappe.top

R. Bash 专题
来源：http://kmi.yj202588.top

================================================================================
来源：http://yii.gogol.net.cn

[R01] shebang 与严格模式
来源：http://myo.yj20258.top

#!/usr/bin/env bash
来源：http://nnd.andypj.xyz

set -euo pipefail
来源：http://idj.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://vci.guannengcc.top

name="Tom"; echo "$name"
来源：http://zsu.epnwcf.com

[R03] 只读变量
来源：http://ycm.sysykeji.top

readonly PI=3.14
来源：http://zgu.hammf.cn

[R04] 位置参数
来源：http://oaq.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jwn.jinqigufen.top

[R05] 参数默认值
来源：http://shj.jinyuanbaomall.cn

name="${1:-default}"
来源：http://rla.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://rdn.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kpc.sxryk.cn

[R07] if 判断文件
来源：http://uoj.yj202588.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wlt.aibaodan.cn

[R08] 数值比较
来源：http://hby.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://abn.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://vzd.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hvg.gaohongyu789.top

[R10] 正则匹配
来源：http://bwq.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dus.ehwqpu.com

[R11] case 多分支
来源：http://cvl.jyoumei.cn

case "$1" in
来源：http://pif.gzhubu.top

start) echo "启动" ;;
来源：http://zdj.yongpay.top

stop)  echo "停止" ;;
来源：http://diq.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://efa.jinyuanbaomall.cn

esac
来源：http://pyy.nanxuanxn.top

[R12] for 遍历文件
来源：http://jvr.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://knj.zdbjq.cn

[R13] for 计数循环
来源：http://pai.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://tyv.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://gqt.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dno.cashguo.top

[R15] while 逐行读文件
来源：http://jgm.mhx1999.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cdu.nanxinkj.top

[R16] until 等待条件
来源：http://fml.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qob.fzhhl.top

[R17] 数组定义与取值
来源：http://hbu.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://don.wangshuangyany.cn

[R18] 遍历数组
来源：http://cyg.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://euc.shzxlz.cn

[R19] 数组长度
来源：http://hli.jqgufenzy.top

echo "${#arr[@]}"
来源：http://luz.mhx1999.top

[R20] 关联数组（字典）
来源：http://huh.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lvf.yj202588.top

[R21] 字符串长度
来源：http://gek.yonumen.top

echo "${#s}"
来源：http://ndy.wangdashe.top

[R22] 截取子串
来源：http://nuw.wangdashe.top

echo "${s:0:5}"
来源：http://zfz.sjlbkw.cn

[R23] 字符串替换
来源：http://uck.sufxvd.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://haz.vehdjk.com

[R24] 大小写转换
来源：http://ixa.hnxiangtu.top

echo "${s^^}"; echo "${s,,}"
来源：http://fpq.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://brm.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vsj.fehbvm.com

[R26] 命令替换
来源：http://nes.jyoumei.cn

now=$(date +%F); echo "$now"
来源：http://bqf.gzhubu.top

[R27] 算术展开
来源：http://wtk.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://rwb.yueranfly.top

[R28] 浮点运算
来源：http://cex.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://qzj.haohaochexian.top

[R29] 定义函数
来源：http://xlf.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vly.hammf.cn

[R30] 函数返回状态码
来源：http://bmb.cheryme.top

f() { return 0; }; f || echo "失败了"
来源：http://vtz.yfazqb.com

[R31] 局部变量
来源：http://brl.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://ygq.cdnleiting.top

[R32] 参数个数校验
来源：http://lmr.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zzu.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://jkb.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wia.dianchejie.cn

[R34] 退出时清理
来源：http://piu.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://upl.haohaochexian.top

[R35] 后台执行并等待
来源：http://rjv.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ahp.yangfankeji.com

[R36] 并发执行多个任务
来源：http://aea.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ebr.yj202588.top

[R37] 把输出赋给变量
来源：http://gct.jinqigufen.top

files=$(ls -1)
来源：http://ejs.52xcode.cn

[R38] 管道串联
来源：http://dxl.cheryme.top

cat a.txt | grep -i error | wc -l
来源：http://rap.tarul.cn

[R39] 重定向标准输出与错误
来源：http://dmt.ivvv.top

cmd > out.log 2>&1
来源：http://jax.yj20258.top

[R40] 追加写日志
来源：http://qqf.epnwcf.com

echo "log" >> out.log
来源：http://wvn.ydzc1.top

[R41] 丢弃输出
来源：http://qgw.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://bgf.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://jyn.yangfankeji.com

wc -l < a.txt
来源：http://hvr.c1oappe.top

[R43] 按名字查找文件
来源：http://ssw.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://cud.shuidangran.top

[R44] 按修改时间查找
来源：http://mme.zdqjudy.top

find . -mtime -7 -type f
来源：http://tbs.c1oappe.top

[R45] 批量删除
来源：http://edz.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://lyd.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://ukm.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jep.hnxiangtu.top

[R47] sed 单行替换
来源：http://zcf.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ifc.nanxuanxn.top

[R48] awk 取指定列
来源：http://rvw.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://ltz.jiagoushi.top

[R49] awk 带条件
来源：http://dmd.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://srz.yuxming.cn

[R50] awk 求和
来源：http://xme.nanxuanxn.top

awk '{s += $2} END {print s}' a.txt
来源：http://los.pycfn.com

[R51] 排序去重取前几
来源：http://esm.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://axb.jinqigfzy.top

[R52] 统计行数
来源：http://kud.xingfuxueyuan.xyz

wc -l a.txt
来源：http://ymd.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://fov.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yeb.zhijiandao.cn

[R54] 比较两个文件
来源：http://umr.xuanzx.com

diff a.txt b.txt
来源：http://dso.gzhubu.top

[R55] 压缩与解压
来源：http://iyo.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rts.yj20258.top

[R56] 远程拷贝
来源：http://rtc.shuidangran.top

scp file user@host:/path/
来源：http://kcq.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://pgu.aibaodan.cn

ssh user@host 'uptime'
来源：http://tsy.wangshuangyany.cn

[R58] 下载文件
来源：http://dul.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sjr.nanxuanxn.top

[R59] 发 POST JSON
来源：http://jnd.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://khu.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://wqh.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hlo.wangdashe.top

[R61] 磁盘占用
来源：http://nuj.gogol.net.cn

df -h;  du -sh *
来源：http://wbs.wangdashe.top

[R62] 找最占空间的文件
来源：http://sbr.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://myi.tianlin.xyz

[R63] 内存与进程
来源：http://vok.ivvv.top

free -h;  ps aux | grep nginx
来源：http://sxm.hywenlv.cn

[R64] 结束进程
来源：http://ghp.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://zdt.gzhubu.top

[R65] 查看端口占用
来源：http://dhk.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pgn.hnxiangtu.top

[R66] 定时任务
来源：http://dzr.yonumen.top

crontab -e;  crontab -l
来源：http://omn.guannengcc.top

[R67] 生成随机十六进制串
来源：http://shh.jianghu66.top

openssl rand -hex 16
来源：http://pul.svipenyu.cn

[R68] 计算文件校验值
来源：http://osi.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ilj.sxryk.cn

[R69] 生成随机密码
来源：http://mgj.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://spi.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://sef.9152youxi.cn

date +%s;  date -d @1700000000
来源：http://syh.zycfv.cn

[R71] 日期格式化
来源：http://iat.hnqzz.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oim.fehbvm.com

[R72] 等待端口就绪
来源：http://vbh.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fmc.shzxlz.cn

[R73] 分割大日志
来源：http://xly.pycfn.com

split -l 1000 big.log part_
来源：http://guq.svipenyu.cn

[R74] 批量重命名
来源：http://osk.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bjn.fengsongda.top

[R75] 导出环境变量
来源：http://nhe.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://sjl.yj202588.top

[R76] 使用临时文件
来源：http://sod.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ruc.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://qjb.guannengcc.top

read -rp "请输入: " ans
来源：http://jqm.daxiang520.top

[R78] 交互式菜单
来源：http://rgw.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bsl.xziqi.cn

[R79] 解析命令行选项
来源：http://fjc.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ckh.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://ukc.0kj1m.cn

time ./run.sh
来源：http://xvt.9152youxi.cn

================================================================================
来源：http://vvg.fengsongda.top

S. C / C++ 专题
来源：http://ohd.xuetiantiany.cn

================================================================================
来源：http://qvu.xuanzx.com

[S01] C：Hello World
来源：http://kef.fanxiaobao.xyz

#include <stdio.h>
来源：http://can.kuanghao11.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xmr.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://hgg.ydzc1.top

int a = 10; printf("%d\n", a);
来源：http://bhj.nwbrower.top

[S03] C：读入整数
来源：http://jfx.ybcxt.top

int x; scanf("%d", &x);
来源：http://uiy.jianghu66.top

[S04] C：字符串复制
来源：http://yay.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dcn.vqdsnc.cn

[S05] C：字符串长度
来源：http://esi.bjfxy.top

strlen(s)
来源：http://gzz.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://vpe.xziqi.cn

strcmp(a, b) == 0
来源：http://odp.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://qds.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gum.sweek.top

[S08] C：动态内存分配与释放
来源：http://gov.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://shc.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://neu.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://scq.yangfankeji.com

[S10] C：指针与解引用
来源：http://ycc.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://hts.hnxiangtu.top

[S11] C：逐行读文件
来源：http://wfq.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://lbw.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bqo.svipenyu.cn

fclose(f);
来源：http://vxe.dianchejie.cn

[S12] C：写文件
来源：http://avc.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kbn.xziqi.cn

[S13] C：宏定义
来源：http://dyl.yanxiufei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yka.quarkkingdee.top

[S14] C：枚举
来源：http://bie.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://prc.bjfxy.top

[S15] C：类型转换
来源：http://bwq.guannengcc.top

(double) a / b
来源：http://mhj.ydjk.org.cn

[S16] C：位操作置位
来源：http://hng.ctjpmb.com

x |= (1 << 3);
来源：http://rgm.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://ryr.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lwz.yuanzhike.top

[S18] C：命令行参数
来源：http://gyk.yonumen.top

int main(int argc, char **argv)
来源：http://pdl.hywenlv.cn

[S19] C：快速排序
来源：http://urq.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://qyk.zycfv.cn

[S20] C：二分查找
来源：http://jrn.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bqj.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://yqn.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pjc.gogol.net.cn

[S22] C：字符串转数字
来源：http://igw.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://fbe.yueranfly.top

[S23] C：随机数
来源：http://ltg.feifeiyinyue.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vxs.wangdashe.top

[S24] C：获取本地时间
来源：http://nkg.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://okv.nanxuanxn.top

[S25] C：内存拷贝
来源：http://jfq.aizwys.cn

memcpy(dst, src, n);
来源：http://ewj.haohaochexian.top

[S26] C：内存清零
来源：http://rwk.hcnkem.com

memset(a, 0, sizeof a);
来源：http://ayh.guannengcc.top

[S27] C：定义常量
来源：http://jcl.chenjidiqi.icu

const double PI = 3.14159;
来源：http://buz.hywenlv.cn

[S28] C：静态变量
来源：http://het.daria6918.cn

static int counter = 0;
来源：http://ucu.yj202588.top

[S29] C：变参函数
来源：http://ebx.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fli.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://fgg.sjlbkw.cn

#ifndef X_H
来源：http://lsw.ydjk.org.cn

#define X_H
来源：http://pca.xingfuxueyuan.xyz

#endif
来源：http://tzr.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://feo.zhoulong.xyz

#include <iostream>
来源：http://gtf.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://yod.hnqzz.top

[S32] C++：字符串
来源：http://xxv.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://awb.quarkkingdee.top

[S33] C++：vector 增删
来源：http://lfa.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uoj.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://gwp.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://mwu.jinqigfzy.top

[S35] C++：map
来源：http://ahb.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ist.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://tkf.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ggm.snrcjt.cn


<!-- 参考信息 -->