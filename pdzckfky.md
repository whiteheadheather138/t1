代发 wailian999

[Q67] 设置隔离级别
来源：http://psd.havefunace.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ttu.sufxvd.cn

[Q68] 保存点
来源：http://aqu.cheryme.top

SAVEPOINT sp1;
来源：http://tav.bjfxy.top

ROLLBACK TO sp1;
来源：http://upg.svipenyu.cn

[Q69] 查看执行计划
来源：http://ycc.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lde.jqgfzy.top

[Q70] 更新统计信息
来源：http://dfx.aizwys.cn

ANALYZE TABLE users;
来源：http://onx.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://exy.guannengcc.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pug.zhiwuduotai.top

[Q72] 查看索引
来源：http://cip.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://ova.uphjek.com

[Q73] 查看表状态
来源：http://zxh.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lvj.tianlin.xyz

[Q74] 强制使用索引
来源：http://mor.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wot.zhengqikj.top

[Q75] 日期格式化
来源：http://znj.shuidangran.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nwt.meibo888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qrg.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://tsh.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fdv.xinyue.icu

[Q77] 时间加减
来源：http://dfk.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rzz.yuxming.cn

[Q78] 当前时间
来源：http://zja.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aai.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://txm.cashguo.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://srz.zhoulong.xyz

[Q80] 字符串截取
来源：http://fhg.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ete.hysaishi.cn

[Q81] 字符串替换
来源：http://wfu.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ckg.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://ulh.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uxm.birdmap.top

[Q83] 大小写转换
来源：http://gog.xziqi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oyv.sysykeji.top

[Q84] 去除首尾空格
来源：http://uuj.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://ccp.jlsjyb.cn

[Q85] 数值取整
来源：http://gzh.c1oappe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ora.hysaishi.cn

[Q86] 读取 JSON 字段
来源：http://uvc.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rhq.tian-w.cn

[Q87] JSON 字段做条件
来源：http://uvx.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://str.hesvh.cn

[Q88] 行转列（条件聚合）
来源：http://aze.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qef.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bfo.jinqigufen.top

[Q89] 判断表是否存在
来源：http://fpu.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ssq.daxiang520.top

[Q90] 生成序号列
来源：http://mwk.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vll.fengsongda.top

================================================================================
来源：http://lgk.zhijiandao.cn

R. Bash 专题
来源：http://kkw.yonumen.top

================================================================================
来源：http://cvd.sufxvd.cn

[R01] shebang 与严格模式
来源：http://tld.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://ufd.yonumen.top

set -euo pipefail
来源：http://nvh.iojbl.cn

[R02] 变量赋值与使用
来源：http://cpq.birdmap.top

name="Tom"; echo "$name"
来源：http://okd.jlsjyb.cn

[R03] 只读变量
来源：http://xaw.tanke756.top

readonly PI=3.14
来源：http://qyj.havefunace.top

[R04] 位置参数
来源：http://xej.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bqa.feifeiyinyue.top

[R05] 参数默认值
来源：http://ekw.zhaomingkeji.xyz

name="${1:-default}"
来源：http://ihq.hesvh.cn

[R06] 判断命令是否存在
来源：http://uzc.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xip.sxryk.cn

[R07] if 判断文件
来源：http://klr.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mss.yuanzhike.top

[R08] 数值比较
来源：http://ngh.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qmy.epnwcf.com

[R09] 字符串比较
来源：http://dji.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mga.yj20258.top

[R10] 正则匹配
来源：http://iiq.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gqe.yfazqb.com

[R11] case 多分支
来源：http://xpb.jiagoushi.top

case "$1" in
来源：http://wsq.tian-w.cn

start) echo "启动" ;;
来源：http://ilj.guowangkeji.top

stop)  echo "停止" ;;
来源：http://rrf.fengsongda.top

*)     echo "未知命令" ;;
来源：http://fmv.cdnleiting.top

esac
来源：http://ugi.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://oqg.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://kjl.cheryme.top

[R13] for 计数循环
来源：http://knx.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://bcz.xinyue.icu

[R14] C 风格 for
来源：http://tuj.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ova.yj20258888.top

[R15] while 逐行读文件
来源：http://vui.kuanghao11.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cmq.hfpthk.cn

[R16] until 等待条件
来源：http://ejb.nwbrower.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fun.hnxiangtu.top

[R17] 数组定义与取值
来源：http://bhm.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yhj.fengsongda.top

[R18] 遍历数组
来源：http://twu.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hro.yvedp.cn

[R19] 数组长度
来源：http://wsc.gogol.net.cn

echo "${#arr[@]}"
来源：http://dcz.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://ysm.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zvw.guannengcc.top

[R21] 字符串长度
来源：http://pps.redwolf501.top

echo "${#s}"
来源：http://ztb.yangfankeji.com

[R22] 截取子串
来源：http://jgd.jlsjyb.cn

echo "${s:0:5}"
来源：http://adt.nwbrower.top

[R23] 字符串替换
来源：http://hhb.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kov.fktsv.cn

[R24] 大小写转换
来源：http://fsd.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://jmu.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://mlp.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://bbt.kuanghao11.cn

[R26] 命令替换
来源：http://kvt.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://fex.xuetiantiany.cn

[R27] 算术展开
来源：http://hqg.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://xto.tanke756.top

[R28] 浮点运算
来源：http://tzu.fzhhl.top

echo "scale=2; 10/3" | bc
来源：http://jmp.jinqigufen.top

[R29] 定义函数
来源：http://gob.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jrj.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://cbz.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://opo.yonumen.top

[R31] 局部变量
来源：http://pzp.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://lmq.cashguo.top

[R32] 参数个数校验
来源：http://qag.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wgy.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://sub.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eoy.cucudq.cn

[R34] 退出时清理
来源：http://mpl.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://cqy.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://sfb.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sti.zycfv.cn

[R36] 并发执行多个任务
来源：http://zkj.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aeb.mhx1999.top

[R37] 把输出赋给变量
来源：http://tzi.snrcjt.cn

files=$(ls -1)
来源：http://arl.shanyushiyangtech.top

[R38] 管道串联
来源：http://nuk.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://ahm.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://uwe.nanxinkj.top

cmd > out.log 2>&1
来源：http://omx.316326.xyz

[R40] 追加写日志
来源：http://azq.fktsv.cn

echo "log" >> out.log
来源：http://veo.ctjpmb.com

[R41] 丢弃输出
来源：http://pog.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://wld.vehdjk.com

[R42] 输入重定向
来源：http://ztq.yj20258.top

wc -l < a.txt
来源：http://wjl.zhiwuduotai.top

[R43] 按名字查找文件
来源：http://hqv.cheryme.top

find . -name "*.log" -type f
来源：http://spk.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://rhv.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://jpz.cheryme.top

[R45] 批量删除
来源：http://zsl.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://vjm.sweek.top

[R46] 递归替换文件内容
来源：http://scq.sufxvd.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://anw.yongpay.top

[R47] sed 单行替换
来源：http://qha.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://bmg.hnqzz.top

[R48] awk 取指定列
来源：http://oae.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://hjy.tian-w.cn

[R49] awk 带条件
来源：http://vhj.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bhr.gotoacloud.top

[R50] awk 求和
来源：http://xpv.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://lrg.cqqwz.cn

[R51] 排序去重取前几
来源：http://szs.wangshuangyany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yak.quarkkingdee.top

[R52] 统计行数
来源：http://url.zycfv.cn

wc -l a.txt
来源：http://jik.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://hnh.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ikb.gzhubu.top

[R54] 比较两个文件
来源：http://yai.hammf.cn

diff a.txt b.txt
来源：http://wyf.ivvv.top

[R55] 压缩与解压
来源：http://yvh.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hqu.xziqi.cn

[R56] 远程拷贝
来源：http://qqr.chenzaomai.com

scp file user@host:/path/
来源：http://jys.shangyingyoupin.top

[R57] 远程执行命令
来源：http://kzw.fehbvm.com

ssh user@host 'uptime'
来源：http://reu.vehdjk.com

[R58] 下载文件
来源：http://zam.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ffc.ppjwa.cn

[R59] 发 POST JSON
来源：http://mse.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sxj.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://zxt.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tem.jqgfzy.top

[R61] 磁盘占用
来源：http://gbh.andypj.xyz

df -h;  du -sh *
来源：http://zmk.guannengcc.top

[R62] 找最占空间的文件
来源：http://yrw.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://jsw.jianghu66.top

[R63] 内存与进程
来源：http://lqj.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://dcd.tian-w.cn

[R64] 结束进程
来源：http://xtf.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://sqw.fzhhl.top

[R65] 查看端口占用
来源：http://ctx.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jac.sjlbkw.cn

[R66] 定时任务
来源：http://gjq.yueranfly.top

crontab -e;  crontab -l
来源：http://eqs.ybcxt.top

[R67] 生成随机十六进制串
来源：http://efo.uphjek.com

openssl rand -hex 16
来源：http://wak.zycfv.cn

[R68] 计算文件校验值
来源：http://dxw.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yas.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://qzq.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://lrl.chenlongwang.top

[R70] 时间戳与互转
来源：http://gdl.sysykeji.top

date +%s;  date -d @1700000000
来源：http://hgc.0kj1m.cn

[R71] 日期格式化
来源：http://jee.chenjidiqi.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://rod.andypj.xyz

[R72] 等待端口就绪
来源：http://shn.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yfj.tian-w.cn

[R73] 分割大日志
来源：http://psn.ppjwa.cn

split -l 1000 big.log part_
来源：http://tzl.xuetiantiany.cn

[R74] 批量重命名
来源：http://arg.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zkd.zdbjq.cn

[R75] 导出环境变量
来源：http://bus.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://zir.iojbl.cn

[R76] 使用临时文件
来源：http://adx.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nle.dianchejie.cn

[R77] 读取用户输入
来源：http://snu.fktsv.cn

read -rp "请输入: " ans
来源：http://fjd.cheryme.top

[R78] 交互式菜单
来源：http://nfq.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://aqv.yj202588.top

[R79] 解析命令行选项
来源：http://eff.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qpr.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://mcu.hywenlv.cn

time ./run.sh
来源：http://znk.bbcook.cn

================================================================================
来源：http://elt.smart0.xyz

S. C / C++ 专题
来源：http://fhv.shanyushiyangtech.top

================================================================================
来源：http://dux.sxryk.cn

[S01] C：Hello World
来源：http://sdm.wangdashe.top

#include <stdio.h>
来源：http://wxh.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xde.wangdashe.top

[S02] C：变量与格式化输出
来源：http://wyv.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://dlk.vqdsnc.cn

[S03] C：读入整数
来源：http://goq.yj202588.top

int x; scanf("%d", &x);
来源：http://mmv.hysaishi.cn

[S04] C：字符串复制
来源：http://wvk.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://fxd.nwbrower.top

[S05] C：字符串长度
来源：http://fiu.guowangkeji.top

strlen(s)
来源：http://ltn.tarul.cn

[S06] C：字符串比较
来源：http://jbr.sweek.top

strcmp(a, b) == 0
来源：http://qsn.fengsongda.top

[S07] C：数组遍历求和
来源：http://mbm.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uiv.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://fky.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qgi.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://lrv.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qkb.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://eal.316326.xyz

int *p = &a;  *p = 5;
来源：http://pzl.smart0.xyz

[S11] C：逐行读文件
来源：http://mrk.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://wsu.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://skc.jinqigfzy.top

fclose(f);
来源：http://wpo.pycfn.com

[S12] C：写文件
来源：http://whx.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lsf.daria6918.cn

[S13] C：宏定义
来源：http://trh.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cvj.zdbjq.cn

[S14] C：枚举
来源：http://uog.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://gmf.ivvv.top

[S15] C：类型转换
来源：http://gxr.xziqi.cn

(double) a / b
来源：http://orv.kuanghao11.cn

[S16] C：位操作置位
来源：http://xxr.sufxvd.cn

x |= (1 << 3);
来源：http://kbd.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://tws.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sbu.jiagoushi.top

[S18] C：命令行参数
来源：http://dvf.uphjek.com

int main(int argc, char **argv)
来源：http://qfu.dianchejie.cn

[S19] C：快速排序
来源：http://lgg.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://nej.pengpengdd.cyou

[S20] C：二分查找
来源：http://vba.shzxlz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ldh.smart0.xyz

[S21] C：字符类别判断
来源：http://hue.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://utn.9152youxi.cn

[S22] C：字符串转数字
来源：http://oqo.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://lcc.dianchejie.cn

[S23] C：随机数
来源：http://kdd.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zll.dashuyun.cn

[S24] C：获取本地时间
来源：http://lsr.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jpm.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://vgk.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://lbq.vqdsnc.cn

[S26] C：内存清零
来源：http://osr.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://zbz.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://nwt.bbcook.cn

const double PI = 3.14159;
来源：http://duq.ydzc1.top

[S28] C：静态变量
来源：http://aut.ydzc1.top

static int counter = 0;
来源：http://pjr.jinqigufen.top

[S29] C：变参函数
来源：http://cxr.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nmj.uphjek.com

[S30] C：头文件保护
来源：http://gmf.316326.xyz

#ifndef X_H
来源：http://iiw.havefunace.top

#define X_H
来源：http://tbf.tarul.cn

#endif
来源：http://fkt.9152youxi.cn

[S31] C++：Hello World
来源：http://pha.havefunace.top

#include <iostream>
来源：http://klp.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://tnt.birdmap.top

[S32] C++：字符串
来源：http://vrf.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://zxu.cashguo.top

[S33] C++：vector 增删
来源：http://krs.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://seb.sufxvd.cn

[S34] C++：遍历 vector
来源：http://hrb.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://lzo.quarkkingdee.top

[S35] C++：map
来源：http://fot.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pyo.cqqwz.cn

[S36] C++：unordered_map
来源：http://mnr.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zye.9152youxi.cn


<!-- 参考信息 -->