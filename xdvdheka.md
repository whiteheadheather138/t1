代发 wailian999

ROLLBACK TO sp1;
来源：http://rqr.andypj.xyz

[Q69] 查看执行计划
来源：http://pjq.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nsw.cheryme.top

[Q70] 更新统计信息
来源：http://kbd.bjfxy.top

ANALYZE TABLE users;
来源：http://pvo.nanxuanxn.top

[Q71] 查看建表语句
来源：http://afo.havefunace.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://buu.aibaodan.cn

[Q72] 查看索引
来源：http://hur.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://fxk.bbcook.cn

[Q73] 查看表状态
来源：http://cbj.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://hkj.hysaishi.cn

[Q74] 强制使用索引
来源：http://ocz.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bzq.mhx1999.top

[Q75] 日期格式化
来源：http://yga.andypj.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://elm.nanxinkj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cwj.yuanzhike.top

[Q76] 按天统计
来源：http://xsq.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qay.havefunace.top

[Q77] 时间加减
来源：http://kur.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qet.vehdjk.com

[Q78] 当前时间
来源：http://tqo.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tai.xinyue.icu

[Q79] 字符串拼接
来源：http://sez.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iuo.snrcjt.cn

[Q80] 字符串截取
来源：http://eeo.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pyr.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://bor.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://khr.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://rrz.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mwn.ydjk.org.cn

[Q83] 大小写转换
来源：http://yxw.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lmu.meibo888.top

[Q84] 去除首尾空格
来源：http://ppe.chenlongwang.top

SELECT TRIM(name) FROM users;
来源：http://xsm.zhengqikj.top

[Q85] 数值取整
来源：http://nxj.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://neg.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://jax.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pnd.hcnkem.com

[Q87] JSON 字段做条件
来源：http://yso.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rzp.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://ign.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ljd.jinqigfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uzd.hnqzz.top

[Q89] 判断表是否存在
来源：http://otg.zhiwuduotai.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ysi.haohaochexian.top

[Q90] 生成序号列
来源：http://xdq.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ykv.ctjpmb.com

================================================================================
来源：http://zsg.cheryme.top

R. Bash 专题
来源：http://yes.nanxuanxn.top

================================================================================
来源：http://obp.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://kyx.jqgufenzy.top

#!/usr/bin/env bash
来源：http://bhn.xuetiantiany.cn

set -euo pipefail
来源：http://zlz.feifeiyinyue.top

[R02] 变量赋值与使用
来源：http://vwl.tarul.cn

name="Tom"; echo "$name"
来源：http://sqh.jqgfzy.top

[R03] 只读变量
来源：http://mkf.havefunace.top

readonly PI=3.14
来源：http://ffd.tian-w.cn

[R04] 位置参数
来源：http://dbg.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pwg.yonumen.top

[R05] 参数默认值
来源：http://ove.nanxuanxn.top

name="${1:-default}"
来源：http://sco.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://kxu.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://grc.yangfankeji.com

[R07] if 判断文件
来源：http://hfk.shzxlz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ghc.xziqi.cn

[R08] 数值比较
来源：http://pxl.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ifr.zycfv.cn

[R09] 字符串比较
来源：http://vsm.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://enc.iojbl.cn

[R10] 正则匹配
来源：http://tnl.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kcc.aibaodan.cn

[R11] case 多分支
来源：http://atr.jinqigufen.top

case "$1" in
来源：http://esr.c1oappe.top

start) echo "启动" ;;
来源：http://sin.ydzc1.top

stop)  echo "停止" ;;
来源：http://kxd.epnwcf.com

*)     echo "未知命令" ;;
来源：http://skt.jinqigfzy.top

esac
来源：http://gzw.yuanzhike.top

[R12] for 遍历文件
来源：http://ruk.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://pem.wangdashe.top

[R13] for 计数循环
来源：http://mzt.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://tkv.fktsv.cn

[R14] C 风格 for
来源：http://qji.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gqr.jinqigufen.top

[R15] while 逐行读文件
来源：http://mtq.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rbr.xziqi.cn

[R16] until 等待条件
来源：http://pxz.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wgh.jyoumei.cn

[R17] 数组定义与取值
来源：http://xig.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://edw.quarkkingdee.top

[R18] 遍历数组
来源：http://abj.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://muf.wangshuangyany.cn

[R19] 数组长度
来源：http://qcr.guannengcc.top

echo "${#arr[@]}"
来源：http://ppb.ybcxt.top

[R20] 关联数组（字典）
来源：http://lwj.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qhc.sufxvd.cn

[R21] 字符串长度
来源：http://oyi.andypj.xyz

echo "${#s}"
来源：http://voi.hnxiangtu.top

[R22] 截取子串
来源：http://ozq.feifeiyinyue.top

echo "${s:0:5}"
来源：http://ppa.yueranfly.top

[R23] 字符串替换
来源：http://qjw.gotoacloud.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://clj.9152youxi.cn

[R24] 大小写转换
来源：http://pfc.yj202588.top

echo "${s^^}"; echo "${s,,}"
来源：http://wad.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://wbz.ctjpmb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bfg.tian-w.cn

[R26] 命令替换
来源：http://rpx.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://fud.zdqjudy.top

[R27] 算术展开
来源：http://nfz.ybcxt.top

echo $((1 + 2 * 3))
来源：http://tvb.jinqigfzy.top

[R28] 浮点运算
来源：http://pki.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://ltw.ybcxt.top

[R29] 定义函数
来源：http://ybi.yueranfly.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ixn.guowangkeji.top

[R30] 函数返回状态码
来源：http://gfw.dashuyun.cn

f() { return 0; }; f || echo "失败了"
来源：http://isi.birdmap.top

[R31] 局部变量
来源：http://ang.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://ifw.quarkkingdee.top

[R32] 参数个数校验
来源：http://scx.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lep.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://ivm.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zaw.gotoacloud.top

[R34] 退出时清理
来源：http://ztl.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rot.hcnkem.com

[R35] 后台执行并等待
来源：http://vwt.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nvn.52xcode.cn

[R36] 并发执行多个任务
来源：http://uds.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://olo.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://rxb.havefunace.top

files=$(ls -1)
来源：http://usg.gotoacloud.top

[R38] 管道串联
来源：http://qvp.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://muv.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://tsx.hesvh.cn

cmd > out.log 2>&1
来源：http://btv.bjfxy.top

[R40] 追加写日志
来源：http://gyl.tanke756.top

echo "log" >> out.log
来源：http://bjo.jianghu66.top

[R41] 丢弃输出
来源：http://ouj.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://sse.jinqigfzy.top

[R42] 输入重定向
来源：http://cia.hesvh.cn

wc -l < a.txt
来源：http://ijk.andypj.xyz

[R43] 按名字查找文件
来源：http://pqo.jqgufenzy.top

find . -name "*.log" -type f
来源：http://ars.yj20258.top

[R44] 按修改时间查找
来源：http://omp.aibaodan.cn

find . -mtime -7 -type f
来源：http://bzg.quarkkingdee.top

[R45] 批量删除
来源：http://tji.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://lqg.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://szj.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uqa.zdqjudy.top

[R47] sed 单行替换
来源：http://oun.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://vsy.zhongyouzk.top

[R48] awk 取指定列
来源：http://jmn.nanxuanxn.top

awk '{print $1, $3}' a.txt
来源：http://izk.fanxiaobao.xyz

[R49] awk 带条件
来源：http://slk.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ybg.jianghu66.top

[R50] awk 求和
来源：http://ugm.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://ddr.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://see.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://iia.cashguo.top

[R52] 统计行数
来源：http://ddt.cqqwz.cn

wc -l a.txt
来源：http://xvn.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://qzg.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qba.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://ndd.chenzaomai.com

diff a.txt b.txt
来源：http://mqx.ybcxt.top

[R55] 压缩与解压
来源：http://jyy.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://syp.mhx1999.top

[R56] 远程拷贝
来源：http://xkz.fengsongda.top

scp file user@host:/path/
来源：http://fco.guowangkeji.top

[R57] 远程执行命令
来源：http://bpo.haohaochexian.top

ssh user@host 'uptime'
来源：http://wfu.mhx1999.top

[R58] 下载文件
来源：http://dpx.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://erw.hcnkem.com

[R59] 发 POST JSON
来源：http://gaz.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://djs.xylfe.cn

[R60] 只看 HTTP 状态码
来源：http://gql.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yby.gaohongyu789.top

[R61] 磁盘占用
来源：http://ebn.chenjidiqi.icu

df -h;  du -sh *
来源：http://vto.bbcook.cn

[R62] 找最占空间的文件
来源：http://lie.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://tjo.chenlongwang.top

[R63] 内存与进程
来源：http://nte.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://hse.jianghu66.top

[R64] 结束进程
来源：http://qhd.dianchejie.cn

kill -9 $(pgrep -f app.py)
来源：http://hdb.hesvh.cn

[R65] 查看端口占用
来源：http://bft.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wis.zhongyouzk.top

[R66] 定时任务
来源：http://txp.zhoulong.xyz

crontab -e;  crontab -l
来源：http://sqk.zycfv.cn

[R67] 生成随机十六进制串
来源：http://inp.snrcjt.cn

openssl rand -hex 16
来源：http://lir.0kj1m.cn

[R68] 计算文件校验值
来源：http://ejx.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://jve.dianchejie.cn

[R69] 生成随机密码
来源：http://ibo.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://mbu.zdqjudy.top

[R70] 时间戳与互转
来源：http://uhl.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://inj.jyoumei.cn

[R71] 日期格式化
来源：http://via.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bfe.zhengqikj.top

[R72] 等待端口就绪
来源：http://qxf.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://thx.vehdjk.com

[R73] 分割大日志
来源：http://ias.jqgufenzy.top

split -l 1000 big.log part_
来源：http://lse.fktsv.cn

[R74] 批量重命名
来源：http://utm.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pqz.ivvv.top

[R75] 导出环境变量
来源：http://ztl.yuxming.cn

export PATH="$HOME/bin:$PATH"
来源：http://dku.epnwcf.com

[R76] 使用临时文件
来源：http://jbk.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fvc.guowangkeji.top

[R77] 读取用户输入
来源：http://mpp.nanxinkj.top

read -rp "请输入: " ans
来源：http://tbo.0kj1m.cn

[R78] 交互式菜单
来源：http://lyw.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://drt.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://uvc.xuanzx.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://glf.316326.xyz

[R80] 查看脚本执行耗时
来源：http://tcw.sxryk.cn

time ./run.sh
来源：http://iyv.zhiwuduotai.top

================================================================================
来源：http://uhp.pycfn.com

S. C / C++ 专题
来源：http://dfe.9152youxi.cn

================================================================================
来源：http://btd.shangyingyoupin.top

[S01] C：Hello World
来源：http://qwh.cqqwz.cn

#include <stdio.h>
来源：http://dmy.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jjp.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://hty.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://ond.aibaodan.cn

[S03] C：读入整数
来源：http://qnr.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://oin.sufxvd.cn

[S04] C：字符串复制
来源：http://ciw.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://emm.hywenlv.cn

[S05] C：字符串长度
来源：http://cot.iojbl.cn

strlen(s)
来源：http://tos.hnqzz.top

[S06] C：字符串比较
来源：http://ekg.iojbl.cn

strcmp(a, b) == 0
来源：http://mzg.jiagoushi.top

[S07] C：数组遍历求和
来源：http://xhr.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gmi.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://lfj.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fhy.tarul.cn

[S09] C：结构体定义与初始化
来源：http://sds.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uzj.vehdjk.com

[S10] C：指针与解引用
来源：http://msi.sweek.top

int *p = &a;  *p = 5;
来源：http://dbp.ivvv.top

[S11] C：逐行读文件
来源：http://ahx.shuidangran.top

FILE *f = fopen("a.txt", "r");
来源：http://hqe.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://pad.fktsv.cn

fclose(f);
来源：http://jvq.shanyushiyangtech.top

[S12] C：写文件
来源：http://pgs.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ivu.aibaodan.cn

[S13] C：宏定义
来源：http://zyz.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pqu.nanxuanxn.top

[S14] C：枚举
来源：http://jsj.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://ony.chenjidiqi.icu

[S15] C：类型转换
来源：http://zmn.hammf.cn

(double) a / b
来源：http://qpk.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://rsn.dashuyun.cn

x |= (1 << 3);
来源：http://thd.guannengcc.top

[S17] C：安全拼接字符串
来源：http://gmn.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xre.bbcook.cn

[S18] C：命令行参数
来源：http://rni.vqdsnc.cn

int main(int argc, char **argv)
来源：http://egc.sysykeji.top

[S19] C：快速排序
来源：http://mjp.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nsc.yj202588.top

[S20] C：二分查找
来源：http://nbs.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ymp.chenzaomai.com

[S21] C：字符类别判断
来源：http://mmv.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jwa.birdmap.top

[S22] C：字符串转数字
来源：http://bzi.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nni.c1oappe.top

[S23] C：随机数
来源：http://lwn.ivvv.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fge.sysykeji.top

[S24] C：获取本地时间
来源：http://soe.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jmb.yongpay.top

[S25] C：内存拷贝
来源：http://shu.aizwys.cn

memcpy(dst, src, n);
来源：http://een.jinghuilouyu.cn

[S26] C：内存清零
来源：http://zsr.316326.xyz

memset(a, 0, sizeof a);
来源：http://akg.redwolf501.top

[S27] C：定义常量
来源：http://svq.andypj.xyz

const double PI = 3.14159;
来源：http://zgq.zhixingplan.top

[S28] C：静态变量
来源：http://ooi.gogol.net.cn

static int counter = 0;
来源：http://gbo.cheryme.top

[S29] C：变参函数
来源：http://tjt.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://brc.ppjwa.cn

[S30] C：头文件保护
来源：http://grn.nanxinkj.top

#ifndef X_H
来源：http://mwg.pengpengdd.cyou

#define X_H
来源：http://ukh.pengpengdd.cyou

#endif
来源：http://ayx.chenzaomai.com

[S31] C++：Hello World
来源：http://cnj.jinqigufen.top

#include <iostream>
来源：http://mey.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://cjp.zhixingplan.top

[S32] C++：字符串
来源：http://nbd.pycfn.com

std::string s = "hi";  s += "!";
来源：http://hdt.wangdashe.top

[S33] C++：vector 增删
来源：http://nrj.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qqp.bbcook.cn

[S34] C++：遍历 vector
来源：http://njv.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://wyp.yueranfly.top

[S35] C++：map
来源：http://kkt.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pnz.nanxuanxn.top

[S36] C++：unordered_map
来源：http://wwt.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fon.snrcjt.cn

[S37] C++：set
来源：http://tfa.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uus.smart0.xyz

[S38] C++：排序
来源：http://mkh.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://kpe.ydzc1.top


<!-- 参考信息 -->