代发 wailian999

ROLLBACK TO sp1;
来源：http://jzd.gzhubu.top

[Q69] 查看执行计划
来源：http://jts.hcnkem.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bjm.zhoulong.xyz

[Q70] 更新统计信息
来源：http://kmx.nanxuanxn.top

ANALYZE TABLE users;
来源：http://crf.iojbl.cn

[Q71] 查看建表语句
来源：http://hgl.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://whq.chenjidiqi.icu

[Q72] 查看索引
来源：http://wqz.quarkkingdee.top

SHOW INDEX FROM users;
来源：http://wig.yuxming.cn

[Q73] 查看表状态
来源：http://jpm.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://upd.andypj.xyz

[Q74] 强制使用索引
来源：http://wxi.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zzd.ppjwa.cn

[Q75] 日期格式化
来源：http://rlp.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ofa.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://upw.jlsjyb.cn

[Q76] 按天统计
来源：http://rcb.yuxming.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vrd.0kj1m.cn

[Q77] 时间加减
来源：http://kdx.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cbn.uphjek.com

[Q78] 当前时间
来源：http://per.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bvs.tian-w.cn

[Q79] 字符串拼接
来源：http://dmc.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jqd.zhiwuduotai.top

[Q80] 字符串截取
来源：http://moc.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tmf.jqgufenzy.top

[Q81] 字符串替换
来源：http://hla.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://stj.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://soh.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ymn.daxiang520.top

[Q83] 大小写转换
来源：http://crg.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gaz.tian-w.cn

[Q84] 去除首尾空格
来源：http://mda.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://rqj.dianchejie.cn

[Q85] 数值取整
来源：http://gmo.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yhl.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://uau.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cag.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://une.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qbo.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://wrj.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hbf.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lxk.hammf.cn

[Q89] 判断表是否存在
来源：http://ysb.jqgfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nth.iojbl.cn

[Q90] 生成序号列
来源：http://ftb.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cqd.tarul.cn

================================================================================
来源：http://rtj.iojbl.cn

R. Bash 专题
来源：http://gib.fzhhl.top

================================================================================
来源：http://jti.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://ugj.nanxinkj.top

#!/usr/bin/env bash
来源：http://kkl.daxiang520.top

set -euo pipefail
来源：http://ded.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://dsv.fzhhl.top

name="Tom"; echo "$name"
来源：http://fha.bjfxy.top

[R03] 只读变量
来源：http://fwn.meibo888.top

readonly PI=3.14
来源：http://uqz.vqdsnc.cn

[R04] 位置参数
来源：http://wzk.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mzt.cheryme.top

[R05] 参数默认值
来源：http://fqi.52xcode.cn

name="${1:-default}"
来源：http://dzi.ivvv.top

[R06] 判断命令是否存在
来源：http://wsg.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nru.sjlbkw.cn

[R07] if 判断文件
来源：http://unp.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lng.jianghu66.top

[R08] 数值比较
来源：http://mkh.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cha.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://kqp.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bpq.chenlongwang.top

[R10] 正则匹配
来源：http://fjs.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fke.xinyue.icu

[R11] case 多分支
来源：http://soi.uphjek.com

case "$1" in
来源：http://ifn.haohaochexian.top

start) echo "启动" ;;
来源：http://dnm.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://byb.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://eis.sxryk.cn

esac
来源：http://dsz.yonumen.top

[R12] for 遍历文件
来源：http://qwk.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://nyw.gzhubu.top

[R13] for 计数循环
来源：http://tqf.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://sdk.mhx1999.top

[R14] C 风格 for
来源：http://ryn.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zrv.xinyue.icu

[R15] while 逐行读文件
来源：http://uks.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xxb.yuanzhike.top

[R16] until 等待条件
来源：http://qor.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gnj.fktsv.cn

[R17] 数组定义与取值
来源：http://xnb.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yxb.nanxuanxn.top

[R18] 遍历数组
来源：http://lhh.fktsv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gxh.xuanzx.com

[R19] 数组长度
来源：http://sri.vqdsnc.cn

echo "${#arr[@]}"
来源：http://hfx.bjfxy.top

[R20] 关联数组（字典）
来源：http://qyh.ywan-chungtsiang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wfm.birdmap.top

[R21] 字符串长度
来源：http://zpf.andypj.xyz

echo "${#s}"
来源：http://gvo.yj202588.top

[R22] 截取子串
来源：http://bbz.zhengqikj.top

echo "${s:0:5}"
来源：http://zfc.wangshuangyany.cn

[R23] 字符串替换
来源：http://ksj.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mqy.zhijiandao.cn

[R24] 大小写转换
来源：http://yvz.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://maf.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://rfr.9152youxi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cju.jqgfzy.top

[R26] 命令替换
来源：http://wmz.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://nfd.zhixingplan.top

[R27] 算术展开
来源：http://ofy.zycfv.cn

echo $((1 + 2 * 3))
来源：http://qbc.ybcxt.top

[R28] 浮点运算
来源：http://bsk.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://tzq.sxryk.cn

[R29] 定义函数
来源：http://dtn.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fxu.wangdashe.top

[R30] 函数返回状态码
来源：http://faw.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://mpw.yj20258888.top

[R31] 局部变量
来源：http://gna.yvedp.cn

f() { local x=1; echo "$x"; }
来源：http://nzp.hnqzz.top

[R32] 参数个数校验
来源：http://aaj.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bjl.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://fsl.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hgv.hesvh.cn

[R34] 退出时清理
来源：http://jtp.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ass.zhongyouzk.top

[R35] 后台执行并等待
来源：http://zyy.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uhx.zdbjq.cn

[R36] 并发执行多个任务
来源：http://kea.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gpy.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://ftb.chenjidiqi.icu

files=$(ls -1)
来源：http://zkj.gogol.net.cn

[R38] 管道串联
来源：http://tgi.xingfuxueyuan.xyz

cat a.txt | grep -i error | wc -l
来源：http://rbz.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://lrd.hfpthk.cn

cmd > out.log 2>&1
来源：http://dvs.xinyue.icu

[R40] 追加写日志
来源：http://guq.hysaishi.cn

echo "log" >> out.log
来源：http://dza.quarkkingdee.top

[R41] 丢弃输出
来源：http://mbg.iojbl.cn

cmd >/dev/null 2>&1
来源：http://ubj.jqgfzy.top

[R42] 输入重定向
来源：http://wqs.cdnleiting.top

wc -l < a.txt
来源：http://ytl.zhoulong.xyz

[R43] 按名字查找文件
来源：http://kuj.quarkkingdee.top

find . -name "*.log" -type f
来源：http://ako.meibo888.top

[R44] 按修改时间查找
来源：http://fbi.hcnkem.com

find . -mtime -7 -type f
来源：http://mrk.yanxiufei.cn

[R45] 批量删除
来源：http://ckv.tarul.cn

find . -name "*.tmp" -delete
来源：http://rlp.hcnkem.com

[R46] 递归替换文件内容
来源：http://hls.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tfy.xuetiantiany.cn

[R47] sed 单行替换
来源：http://blh.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://wfu.ppjwa.cn

[R48] awk 取指定列
来源：http://zqy.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://feg.jqgfzy.top

[R49] awk 带条件
来源：http://msa.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://txj.vqdsnc.cn

[R50] awk 求和
来源：http://mzv.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://trt.zycfv.cn

[R51] 排序去重取前几
来源：http://lbn.quarkkingdee.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hab.jiagoushi.top

[R52] 统计行数
来源：http://rkq.ivvv.top

wc -l a.txt
来源：http://cgi.yongpay.top

[R53] 查看文件头与实时尾
来源：http://owd.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://htv.fehbvm.com

[R54] 比较两个文件
来源：http://vrd.feifeiyinyue.top

diff a.txt b.txt
来源：http://zni.hongshengwenyu.top

[R55] 压缩与解压
来源：http://mzx.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yoz.yanxiufei.cn

[R56] 远程拷贝
来源：http://stu.jianghu66.top

scp file user@host:/path/
来源：http://mqf.feifeiyinyue.top

[R57] 远程执行命令
来源：http://xpg.0kj1m.cn

ssh user@host 'uptime'
来源：http://hgy.ivvv.top

[R58] 下载文件
来源：http://oek.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bfy.tian-w.cn

[R59] 发 POST JSON
来源：http://apj.hfpthk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nja.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://vhz.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iqb.52xcode.cn

[R61] 磁盘占用
来源：http://bxt.ivvv.top

df -h;  du -sh *
来源：http://bzt.guannengcc.top

[R62] 找最占空间的文件
来源：http://ljc.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://xbi.zycfv.cn

[R63] 内存与进程
来源：http://yql.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://ttq.uphjek.com

[R64] 结束进程
来源：http://smy.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://slc.xylfe.cn

[R65] 查看端口占用
来源：http://gqm.ivvv.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xsn.gzhubu.top

[R66] 定时任务
来源：http://lkd.bjfxy.top

crontab -e;  crontab -l
来源：http://yzz.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://nan.yanxiufei.cn

openssl rand -hex 16
来源：http://xhe.iojbl.cn

[R68] 计算文件校验值
来源：http://vsf.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://xig.pengpengdd.cyou

[R69] 生成随机密码
来源：http://npo.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://vjp.vqdsnc.cn

[R70] 时间戳与互转
来源：http://hqh.yuxming.cn

date +%s;  date -d @1700000000
来源：http://pwh.xziqi.cn

[R71] 日期格式化
来源：http://gzo.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mna.xinyue.icu

[R72] 等待端口就绪
来源：http://kzz.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tme.zhoulong.xyz

[R73] 分割大日志
来源：http://gum.nwbrower.top

split -l 1000 big.log part_
来源：http://ida.hammf.cn

[R74] 批量重命名
来源：http://yof.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tnk.redwolf501.top

[R75] 导出环境变量
来源：http://ycp.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://ybv.hammf.cn

[R76] 使用临时文件
来源：http://ynb.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jlv.quarkkingdee.top

[R77] 读取用户输入
来源：http://hfc.9152youxi.cn

read -rp "请输入: " ans
来源：http://ria.shangyingyoupin.top

[R78] 交互式菜单
来源：http://ast.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://und.xziqi.cn

[R79] 解析命令行选项
来源：http://gpz.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ctk.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://aez.tanke756.top

time ./run.sh
来源：http://ijx.daria6918.cn

================================================================================
来源：http://jxr.sxryk.cn

S. C / C++ 专题
来源：http://tka.yj202588.top

================================================================================
来源：http://icw.ivvv.top

[S01] C：Hello World
来源：http://djx.c1oappe.top

#include <stdio.h>
来源：http://qlm.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jre.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://pya.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://ztr.haohaochexian.top

[S03] C：读入整数
来源：http://qjt.ybcxt.top

int x; scanf("%d", &x);
来源：http://xdv.gzhubu.top

[S04] C：字符串复制
来源：http://vci.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mft.tian-w.cn

[S05] C：字符串长度
来源：http://dcm.ywan-chungtsiang.top

strlen(s)
来源：http://kht.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://jjz.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://khn.gzhubu.top

[S07] C：数组遍历求和
来源：http://auo.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ycy.jinqigufen.top

[S08] C：动态内存分配与释放
来源：http://kde.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ljx.sweek.top

[S09] C：结构体定义与初始化
来源：http://wpb.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ztj.redwolf501.top

[S10] C：指针与解引用
来源：http://mwz.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://dyn.bbcook.cn

[S11] C：逐行读文件
来源：http://xzc.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://gep.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jgn.shzxlz.cn

fclose(f);
来源：http://zmg.hcnkem.com

[S12] C：写文件
来源：http://hzg.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dzl.cqqwz.cn

[S13] C：宏定义
来源：http://fka.sufxvd.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dek.fktsv.cn

[S14] C：枚举
来源：http://pzx.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://uje.hnxiangtu.top

[S15] C：类型转换
来源：http://yjn.epnwcf.com

(double) a / b
来源：http://xer.pycfn.com

[S16] C：位操作置位
来源：http://atr.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://uuz.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://nma.fzhhl.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bfr.quarkkingdee.top

[S18] C：命令行参数
来源：http://ozv.andypj.xyz

int main(int argc, char **argv)
来源：http://hlx.dashuyun.cn

[S19] C：快速排序
来源：http://grc.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://arb.yj20258888.top

[S20] C：二分查找
来源：http://ttq.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://myj.hnxiangtu.top

[S21] C：字符类别判断
来源：http://wvf.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gqp.yj20258.top

[S22] C：字符串转数字
来源：http://rur.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://wzz.haohaochexian.top

[S23] C：随机数
来源：http://xxx.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xzp.zdbjq.cn

[S24] C：获取本地时间
来源：http://lvh.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qgq.cheryme.top

[S25] C：内存拷贝
来源：http://kqi.yonumen.top

memcpy(dst, src, n);
来源：http://crj.bbcook.cn

[S26] C：内存清零
来源：http://keu.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://fmd.shangyingyoupin.top

[S27] C：定义常量
来源：http://lfk.xylfe.cn

const double PI = 3.14159;
来源：http://fjd.sjlbkw.cn

[S28] C：静态变量
来源：http://ghu.zhiwuduotai.top

static int counter = 0;
来源：http://loc.zhoulong.xyz

[S29] C：变参函数
来源：http://zrh.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qpv.hammf.cn

[S30] C：头文件保护
来源：http://kto.nanxinkj.top

#ifndef X_H
来源：http://zgk.jyoumei.cn

#define X_H
来源：http://muf.cucudq.cn

#endif
来源：http://knd.yueranfly.top

[S31] C++：Hello World
来源：http://vfq.ctjpmb.com

#include <iostream>
来源：http://gct.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://zsj.yfazqb.com

[S32] C++：字符串
来源：http://uva.ivvv.top

std::string s = "hi";  s += "!";
来源：http://lce.chenlongwang.top

[S33] C++：vector 增删
来源：http://wuy.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kcf.zdbjq.cn

[S34] C++：遍历 vector
来源：http://wrj.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://sha.fanxiaobao.xyz

[S35] C++：map
来源：http://qha.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gwc.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://ygp.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bvh.jianghu66.top

[S37] C++：set
来源：http://ylp.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ntb.ctjpmb.com

[S38] C++：排序
来源：http://cdx.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://zwv.pengpengdd.cyou


<!-- 参考信息 -->