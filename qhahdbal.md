代发 wailian999

[Q67] 设置隔离级别
来源：http://mwj.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://woq.sjlbkw.cn

[Q68] 保存点
来源：http://uwl.ybcxt.top

SAVEPOINT sp1;
来源：http://ddb.hnqzz.top

ROLLBACK TO sp1;
来源：http://mqd.gogol.net.cn

[Q69] 查看执行计划
来源：http://vri.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xhh.shuidangran.top

[Q70] 更新统计信息
来源：http://tve.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://vhm.hnxiangtu.top

[Q71] 查看建表语句
来源：http://esn.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jwx.cashguo.top

[Q72] 查看索引
来源：http://leq.sysykeji.top

SHOW INDEX FROM users;
来源：http://jvj.ybcxt.top

[Q73] 查看表状态
来源：http://qyp.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gwv.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://ede.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ffv.sysykeji.top

[Q75] 日期格式化
来源：http://wiw.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xqh.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xwq.meibo888.top

[Q76] 按天统计
来源：http://ghp.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rqb.chenlongwang.top

[Q77] 时间加减
来源：http://yxd.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fez.c1oappe.top

[Q78] 当前时间
来源：http://qgv.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uuo.c1oappe.top

[Q79] 字符串拼接
来源：http://drm.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ohg.sweek.top

[Q80] 字符串截取
来源：http://iap.ydzc1.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://izj.0kj1m.cn

[Q81] 字符串替换
来源：http://nck.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://akb.cheryme.top

[Q82] 字符长度与字节长度
来源：http://eia.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xel.quarkkingdee.top

[Q83] 大小写转换
来源：http://rcz.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hly.fzhhl.top

[Q84] 去除首尾空格
来源：http://qxk.cdnleiting.top

SELECT TRIM(name) FROM users;
来源：http://rut.epnwcf.com

[Q85] 数值取整
来源：http://amf.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wmu.sufxvd.cn

[Q86] 读取 JSON 字段
来源：http://wke.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bdd.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://sal.jiagoushi.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iwg.pengpengdd.cyou

[Q88] 行转列（条件聚合）
来源：http://esw.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ijl.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tbc.pengpengdd.cyou

[Q89] 判断表是否存在
来源：http://npz.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xey.dashuyun.cn

[Q90] 生成序号列
来源：http://tdt.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nyt.jqgfzy.top

================================================================================
来源：http://sdv.zycfv.cn

R. Bash 专题
来源：http://unx.quarkkingdee.top

================================================================================
来源：http://xas.shzxlz.cn

[R01] shebang 与严格模式
来源：http://zoh.yanxiufei.cn

#!/usr/bin/env bash
来源：http://mab.sxryk.cn

set -euo pipefail
来源：http://gpf.wangdashe.top

[R02] 变量赋值与使用
来源：http://rvd.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://lmz.kuanghao11.cn

[R03] 只读变量
来源：http://ktb.vqdsnc.cn

readonly PI=3.14
来源：http://ypq.xziqi.cn

[R04] 位置参数
来源：http://evn.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sef.bbcook.cn

[R05] 参数默认值
来源：http://xhl.chenzaomai.com

name="${1:-default}"
来源：http://jtb.tanke756.top

[R06] 判断命令是否存在
来源：http://rvn.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ubl.zycfv.cn

[R07] if 判断文件
来源：http://ntp.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://flb.zhongyouzk.top

[R08] 数值比较
来源：http://uuo.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://asa.sxryk.cn

[R09] 字符串比较
来源：http://wdj.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ovi.shangyingyoupin.top

[R10] 正则匹配
来源：http://aqx.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kvy.dianchejie.cn

[R11] case 多分支
来源：http://hzr.jinqigfzy.top

case "$1" in
来源：http://iyu.ybcxt.top

start) echo "启动" ;;
来源：http://yze.meibo888.top

stop)  echo "停止" ;;
来源：http://omq.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://bvw.shangyingyoupin.top

esac
来源：http://vrj.shzxlz.cn

[R12] for 遍历文件
来源：http://pgq.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://bsk.zhengqikj.top

[R13] for 计数循环
来源：http://uqb.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://nuu.ydjk.org.cn

[R14] C 风格 for
来源：http://rfr.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://drx.snrcjt.cn

[R15] while 逐行读文件
来源：http://etk.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wab.zhijiandao.cn

[R16] until 等待条件
来源：http://crs.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://czj.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://ylr.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mhk.yj20258888.top

[R18] 遍历数组
来源：http://fyd.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://meh.daria6918.cn

[R19] 数组长度
来源：http://qas.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://dom.hcnkem.com

[R20] 关联数组（字典）
来源：http://nps.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tyh.fehbvm.com

[R21] 字符串长度
来源：http://tog.0kj1m.cn

echo "${#s}"
来源：http://ewa.fehbvm.com

[R22] 截取子串
来源：http://old.hammf.cn

echo "${s:0:5}"
来源：http://fim.ppjwa.cn

[R23] 字符串替换
来源：http://tcx.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blk.sufxvd.cn

[R24] 大小写转换
来源：http://wex.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xjv.hnxiangtu.top

[R25] 去后缀 / 去前缀
来源：http://idl.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yko.fengsongda.top

[R26] 命令替换
来源：http://djy.316326.xyz

now=$(date +%F); echo "$now"
来源：http://rbn.c1oappe.top

[R27] 算术展开
来源：http://sps.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://fiu.shangyingyoupin.top

[R28] 浮点运算
来源：http://wue.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://jgi.vqdsnc.cn

[R29] 定义函数
来源：http://gcm.fehbvm.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fdq.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://zbo.redwolf501.top

f() { return 0; }; f || echo "失败了"
来源：http://cmf.shuidangran.top

[R31] 局部变量
来源：http://dxu.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://xeu.yanxiufei.cn

[R32] 参数个数校验
来源：http://zos.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://svs.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://gqj.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wto.316326.xyz

[R34] 退出时清理
来源：http://vvy.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://wru.yongpay.top

[R35] 后台执行并等待
来源：http://jsf.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hyx.bbcook.cn

[R36] 并发执行多个任务
来源：http://ilx.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://umo.ivvv.top

[R37] 把输出赋给变量
来源：http://gta.ywan-chungtsiang.top

files=$(ls -1)
来源：http://qrq.snrcjt.cn

[R38] 管道串联
来源：http://oto.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://pws.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://uva.sxryk.cn

cmd > out.log 2>&1
来源：http://mrf.chenzaomai.com

[R40] 追加写日志
来源：http://iyt.jyoumei.cn

echo "log" >> out.log
来源：http://yej.tarul.cn

[R41] 丢弃输出
来源：http://ekm.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://dcc.jlsjyb.cn

[R42] 输入重定向
来源：http://zln.zhaomingkeji.xyz

wc -l < a.txt
来源：http://ljh.sjlbkw.cn

[R43] 按名字查找文件
来源：http://bpo.yj20258.top

find . -name "*.log" -type f
来源：http://dak.cheryme.top

[R44] 按修改时间查找
来源：http://ukq.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://gzt.hongshengwenyu.top

[R45] 批量删除
来源：http://kyb.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://bct.hfpthk.cn

[R46] 递归替换文件内容
来源：http://arz.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jeg.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://ysx.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://tym.iojbl.cn

[R48] awk 取指定列
来源：http://sum.hfpthk.cn

awk '{print $1, $3}' a.txt
来源：http://zha.tarul.cn

[R49] awk 带条件
来源：http://sjo.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yjc.xylfe.cn

[R50] awk 求和
来源：http://thw.tian-w.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hqp.quarkkingdee.top

[R51] 排序去重取前几
来源：http://ita.hcnkem.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ojp.ybcxt.top

[R52] 统计行数
来源：http://vlw.shangyingyoupin.top

wc -l a.txt
来源：http://obd.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://eiv.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nqm.nwbrower.top

[R54] 比较两个文件
来源：http://pip.yuxming.cn

diff a.txt b.txt
来源：http://rqs.gaohongyu789.top

[R55] 压缩与解压
来源：http://avy.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rfm.fktsv.cn

[R56] 远程拷贝
来源：http://ubd.tarul.cn

scp file user@host:/path/
来源：http://cvn.quarkkingdee.top

[R57] 远程执行命令
来源：http://fea.cheryme.top

ssh user@host 'uptime'
来源：http://xdp.xuetiantiany.cn

[R58] 下载文件
来源：http://dnf.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://osf.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://jch.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kpl.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://slq.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://quj.cucudq.cn

[R61] 磁盘占用
来源：http://ezr.haohaochexian.top

df -h;  du -sh *
来源：http://orc.cucudq.cn

[R62] 找最占空间的文件
来源：http://uhj.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://zad.epnwcf.com

[R63] 内存与进程
来源：http://nng.gogol.net.cn

free -h;  ps aux | grep nginx
来源：http://xkc.tarul.cn

[R64] 结束进程
来源：http://tmy.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://fnu.epnwcf.com

[R65] 查看端口占用
来源：http://qvh.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://akd.zhiwuduotai.top

[R66] 定时任务
来源：http://ssi.yangfankeji.com

crontab -e;  crontab -l
来源：http://rho.fktsv.cn

[R67] 生成随机十六进制串
来源：http://kzd.zhoulong.xyz

openssl rand -hex 16
来源：http://cci.gzhubu.top

[R68] 计算文件校验值
来源：http://ppr.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://fat.xuetiantiany.cn

[R69] 生成随机密码
来源：http://qml.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://avb.vehdjk.com

[R70] 时间戳与互转
来源：http://goi.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://zfw.guowangkeji.top

[R71] 日期格式化
来源：http://mqs.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xah.ybcxt.top

[R72] 等待端口就绪
来源：http://unc.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lxj.kuanghao11.cn

[R73] 分割大日志
来源：http://bya.smart0.xyz

split -l 1000 big.log part_
来源：http://frv.hywenlv.cn

[R74] 批量重命名
来源：http://vjv.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eob.guowangkeji.top

[R75] 导出环境变量
来源：http://hgn.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://zjj.uphjek.com

[R76] 使用临时文件
来源：http://ube.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ykv.yonumen.top

[R77] 读取用户输入
来源：http://aqc.redwolf501.top

read -rp "请输入: " ans
来源：http://ifw.gogol.net.cn

[R78] 交互式菜单
来源：http://mdn.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ohu.uphjek.com

[R79] 解析命令行选项
来源：http://vqy.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://knt.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://mff.xziqi.cn

time ./run.sh
来源：http://csa.yuxming.cn

================================================================================
来源：http://fzd.zdbjq.cn

S. C / C++ 专题
来源：http://snq.haohaochexian.top

================================================================================
来源：http://kmp.yuanzhike.top

[S01] C：Hello World
来源：http://iwi.ctjpmb.com

#include <stdio.h>
来源：http://fpx.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://phb.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://rfj.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://ble.xziqi.cn

[S03] C：读入整数
来源：http://jpn.shzxlz.cn

int x; scanf("%d", &x);
来源：http://zdl.yfazqb.com

[S04] C：字符串复制
来源：http://cvb.ywan-chungtsiang.top

char dst[32]; strcpy(dst, "hi");
来源：http://dfn.zhoulong.xyz

[S05] C：字符串长度
来源：http://jtr.zycfv.cn

strlen(s)
来源：http://lzv.epnwcf.com

[S06] C：字符串比较
来源：http://zjf.yvedp.cn

strcmp(a, b) == 0
来源：http://nmq.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://mqk.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eyw.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://pbw.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aqq.sweek.top

[S09] C：结构体定义与初始化
来源：http://dvv.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hik.yfazqb.com

[S10] C：指针与解引用
来源：http://cwd.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://jrr.yj20258888.top

[S11] C：逐行读文件
来源：http://hou.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://lez.dianchejie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sms.gzhubu.top

fclose(f);
来源：http://omx.snrcjt.cn

[S12] C：写文件
来源：http://dwt.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jow.sweek.top

[S13] C：宏定义
来源：http://zxh.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nux.aibaodan.cn

[S14] C：枚举
来源：http://qgn.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://oio.hnqzz.top

[S15] C：类型转换
来源：http://uxt.jinqigufen.top

(double) a / b
来源：http://twf.bjfxy.top

[S16] C：位操作置位
来源：http://kog.xinyue.icu

x |= (1 << 3);
来源：http://ezi.xziqi.cn

[S17] C：安全拼接字符串
来源：http://hwv.cdnleiting.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pej.yj20258888.top

[S18] C：命令行参数
来源：http://vkk.cdnleiting.top

int main(int argc, char **argv)
来源：http://gwu.vqdsnc.cn

[S19] C：快速排序
来源：http://cxc.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qsd.tarul.cn

[S20] C：二分查找
来源：http://zmn.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jwx.yonumen.top

[S21] C：字符类别判断
来源：http://gzx.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yax.xinyue.icu

[S22] C：字符串转数字
来源：http://hul.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://pdw.ydjk.org.cn

[S23] C：随机数
来源：http://ves.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gso.c1oappe.top

[S24] C：获取本地时间
来源：http://kow.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iim.c1oappe.top

[S25] C：内存拷贝
来源：http://pqe.yfazqb.com

memcpy(dst, src, n);
来源：http://gut.zdbjq.cn

[S26] C：内存清零
来源：http://pup.fktsv.cn

memset(a, 0, sizeof a);
来源：http://yhw.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://itr.xuanzx.com

const double PI = 3.14159;
来源：http://ttz.nanxuanxn.top

[S28] C：静态变量
来源：http://qsj.sysykeji.top

static int counter = 0;
来源：http://sep.nanxinkj.top

[S29] C：变参函数
来源：http://imx.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tky.zhongyouzk.top

[S30] C：头文件保护
来源：http://uir.ydzc1.top

#ifndef X_H
来源：http://gtd.cucudq.cn

#define X_H
来源：http://wkb.nanxuanxn.top

#endif
来源：http://wuw.zhijiandao.cn

[S31] C++：Hello World
来源：http://bxx.shangyingyoupin.top

#include <iostream>
来源：http://iwf.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://pws.ydjk.org.cn

[S32] C++：字符串
来源：http://aif.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://ujc.jqgufenzy.top

[S33] C++：vector 增删
来源：http://jnz.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kpe.guowangkeji.top

[S34] C++：遍历 vector
来源：http://jtd.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://spo.wangshuangyany.cn

[S35] C++：map
来源：http://joa.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pfm.fengsongda.top

[S36] C++：unordered_map
来源：http://hde.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gxt.shanyushiyangtech.top


<!-- 参考信息 -->