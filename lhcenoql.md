代发 wailian999

ROLLBACK TO sp1;
来源：http://pcj.ehwqpu.com

[Q69] 查看执行计划
来源：http://usi.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jcl.52xcode.cn

[Q70] 更新统计信息
来源：http://rdm.hesvh.cn

ANALYZE TABLE users;
来源：http://ype.ehwqpu.com

[Q71] 查看建表语句
来源：http://pea.dashuyun.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tog.chenlongwang.top

[Q72] 查看索引
来源：http://xss.c1oappe.top

SHOW INDEX FROM users;
来源：http://cxd.dashuyun.cn

[Q73] 查看表状态
来源：http://sic.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dnb.sysykeji.top

[Q74] 强制使用索引
来源：http://lel.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jmd.nanxinkj.top

[Q75] 日期格式化
来源：http://exb.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mww.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jby.aizwys.cn

[Q76] 按天统计
来源：http://ghv.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bns.nwbrower.top

[Q77] 时间加减
来源：http://vwr.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ofa.yangfankeji.com

[Q78] 当前时间
来源：http://deu.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kfm.nanxuanxn.top

[Q79] 字符串拼接
来源：http://niq.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tzq.xylfe.cn

[Q80] 字符串截取
来源：http://wna.shanyushiyangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sfw.yonumen.top

[Q81] 字符串替换
来源：http://ldb.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kvt.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://ytm.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ykr.jinqigfzy.top

[Q83] 大小写转换
来源：http://yvx.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xjj.pycfn.com

[Q84] 去除首尾空格
来源：http://dxg.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://wom.cucudq.cn

[Q85] 数值取整
来源：http://brq.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tok.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://tzw.jqgfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://urn.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://slm.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jjz.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://bkk.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kmr.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dlq.meibo888.top

[Q89] 判断表是否存在
来源：http://cpc.tarul.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://llp.pycfn.com

[Q90] 生成序号列
来源：http://nvs.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eor.yj202588.top

================================================================================
来源：http://tfc.jlsjyb.cn

R. Bash 专题
来源：http://bxs.ctjpmb.com

================================================================================
来源：http://vzq.bbcook.cn

[R01] shebang 与严格模式
来源：http://wri.hysaishi.cn

#!/usr/bin/env bash
来源：http://vmh.aibaodan.cn

set -euo pipefail
来源：http://ebh.aibaodan.cn

[R02] 变量赋值与使用
来源：http://phm.zycfv.cn

name="Tom"; echo "$name"
来源：http://kft.andypj.xyz

[R03] 只读变量
来源：http://xtf.zdqjudy.top

readonly PI=3.14
来源：http://adq.zhijiandao.cn

[R04] 位置参数
来源：http://ysd.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qrf.zhixingplan.top

[R05] 参数默认值
来源：http://amg.ivvv.top

name="${1:-default}"
来源：http://qsc.316326.xyz

[R06] 判断命令是否存在
来源：http://jkg.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ets.zdbjq.cn

[R07] if 判断文件
来源：http://izh.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aea.jiagoushi.top

[R08] 数值比较
来源：http://pdi.quarkkingdee.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sqm.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://ycd.nwbrower.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ega.tianlin.xyz

[R10] 正则匹配
来源：http://dab.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nfg.jinqigfzy.top

[R11] case 多分支
来源：http://grs.jinqigufen.top

case "$1" in
来源：http://npz.zdqjudy.top

start) echo "启动" ;;
来源：http://vzn.cucudq.cn

stop)  echo "停止" ;;
来源：http://kvd.yuxming.cn

*)     echo "未知命令" ;;
来源：http://yqw.bbcook.cn

esac
来源：http://izg.tarul.cn

[R12] for 遍历文件
来源：http://ewp.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://auy.dashuyun.cn

[R13] for 计数循环
来源：http://bfr.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://edg.shzxlz.cn

[R14] C 风格 for
来源：http://lab.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dni.cashguo.top

[R15] while 逐行读文件
来源：http://gfh.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mho.tianlin.xyz

[R16] until 等待条件
来源：http://dat.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vxz.chenzaomai.com

[R17] 数组定义与取值
来源：http://pzi.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://igr.wangdashe.top

[R18] 遍历数组
来源：http://gqm.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pii.yj20258.top

[R19] 数组长度
来源：http://hom.ybcxt.top

echo "${#arr[@]}"
来源：http://fkp.xinyue.icu

[R20] 关联数组（字典）
来源：http://wag.ctjpmb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pzz.kuanghao11.cn

[R21] 字符串长度
来源：http://gnn.uphjek.com

echo "${#s}"
来源：http://uwh.zycfv.cn

[R22] 截取子串
来源：http://fvn.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://ola.zhijiandao.cn

[R23] 字符串替换
来源：http://dfh.shanyushiyangtech.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nle.daria6918.cn

[R24] 大小写转换
来源：http://gev.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://aci.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://vlz.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eoz.smart0.xyz

[R26] 命令替换
来源：http://ipq.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://juq.tian-w.cn

[R27] 算术展开
来源：http://wsu.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://ihh.yonumen.top

[R28] 浮点运算
来源：http://gry.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://nsy.havefunace.top

[R29] 定义函数
来源：http://slh.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tcu.yuanzhike.top

[R30] 函数返回状态码
来源：http://rhx.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://hqz.uphjek.com

[R31] 局部变量
来源：http://gdd.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://odh.chenlongwang.top

[R32] 参数个数校验
来源：http://qlg.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gvf.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://qci.tianlin.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://twv.guannengcc.top

[R34] 退出时清理
来源：http://qgw.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://rtg.c1oappe.top

[R35] 后台执行并等待
来源：http://szy.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vff.jianghu66.top

[R36] 并发执行多个任务
来源：http://isb.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pzf.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://dbn.jinqigfzy.top

files=$(ls -1)
来源：http://jdd.zhixingplan.top

[R38] 管道串联
来源：http://scq.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://tyq.jlsjyb.cn

[R39] 重定向标准输出与错误
来源：http://qqj.shzxlz.cn

cmd > out.log 2>&1
来源：http://bhw.zdbjq.cn

[R40] 追加写日志
来源：http://bkl.wangdashe.top

echo "log" >> out.log
来源：http://aqz.sufxvd.cn

[R41] 丢弃输出
来源：http://gsb.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://pvr.yonumen.top

[R42] 输入重定向
来源：http://ycs.sufxvd.cn

wc -l < a.txt
来源：http://kko.zdbjq.cn

[R43] 按名字查找文件
来源：http://fcg.yj20258.top

find . -name "*.log" -type f
来源：http://ezt.yanxiufei.cn

[R44] 按修改时间查找
来源：http://zma.hfpthk.cn

find . -mtime -7 -type f
来源：http://pod.tianlin.xyz

[R45] 批量删除
来源：http://kkh.snrcjt.cn

find . -name "*.tmp" -delete
来源：http://imq.jiagoushi.top

[R46] 递归替换文件内容
来源：http://yeh.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rxp.jinqigfzy.top

[R47] sed 单行替换
来源：http://scy.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://zpj.hywenlv.cn

[R48] awk 取指定列
来源：http://jdm.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://rnw.hongshengwenyu.top

[R49] awk 带条件
来源：http://nms.shanyushiyangtech.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cba.ppjwa.cn

[R50] awk 求和
来源：http://wtm.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://slf.52xcode.cn

[R51] 排序去重取前几
来源：http://lyt.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vjn.daxiang520.top

[R52] 统计行数
来源：http://txf.shanyushiyangtech.top

wc -l a.txt
来源：http://dub.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://puq.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pzg.hongshengwenyu.top

[R54] 比较两个文件
来源：http://kdm.nanxinkj.top

diff a.txt b.txt
来源：http://oqk.xuetiantiany.cn

[R55] 压缩与解压
来源：http://pep.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xqd.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://uau.hnqzz.top

scp file user@host:/path/
来源：http://exx.chenjidiqi.icu

[R57] 远程执行命令
来源：http://ryy.fzhhl.top

ssh user@host 'uptime'
来源：http://xao.tanke756.top

[R58] 下载文件
来源：http://ogu.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mcs.cdnleiting.top

[R59] 发 POST JSON
来源：http://xaw.zhixingplan.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://peo.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://pwy.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iua.quarkkingdee.top

[R61] 磁盘占用
来源：http://ovl.sweek.top

df -h;  du -sh *
来源：http://hir.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://kig.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://ept.chenlongwang.top

[R63] 内存与进程
来源：http://aia.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://efa.jinqigfzy.top

[R64] 结束进程
来源：http://bji.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://zkr.hysaishi.cn

[R65] 查看端口占用
来源：http://krq.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sct.snrcjt.cn

[R66] 定时任务
来源：http://enk.jianghu66.top

crontab -e;  crontab -l
来源：http://ioq.yuxming.cn

[R67] 生成随机十六进制串
来源：http://xtz.cqqwz.cn

openssl rand -hex 16
来源：http://vfo.ehwqpu.com

[R68] 计算文件校验值
来源：http://tib.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://bge.gzhubu.top

[R69] 生成随机密码
来源：http://weu.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://krj.xziqi.cn

[R70] 时间戳与互转
来源：http://qva.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://cgn.chenlongwang.top

[R71] 日期格式化
来源：http://lyz.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mua.hysaishi.cn

[R72] 等待端口就绪
来源：http://yth.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nmd.smart0.xyz

[R73] 分割大日志
来源：http://sas.gaohongyu789.top

split -l 1000 big.log part_
来源：http://dtc.haohaochexian.top

[R74] 批量重命名
来源：http://zcq.zhengqikj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mcq.0kj1m.cn

[R75] 导出环境变量
来源：http://ube.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://wyj.xylfe.cn

[R76] 使用临时文件
来源：http://cbb.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zyj.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://fkb.tian-w.cn

read -rp "请输入: " ans
来源：http://quv.xziqi.cn

[R78] 交互式菜单
来源：http://uzj.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://clq.zhoulong.xyz

[R79] 解析命令行选项
来源：http://lev.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://etr.hammf.cn

[R80] 查看脚本执行耗时
来源：http://tji.jlsjyb.cn

time ./run.sh
来源：http://rxd.yfazqb.com

================================================================================
来源：http://xsh.vehdjk.com

S. C / C++ 专题
来源：http://kfx.sysykeji.top

================================================================================
来源：http://tuk.xuetiantiany.cn

[S01] C：Hello World
来源：http://thd.zhiwuduotai.top

#include <stdio.h>
来源：http://hug.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://yyp.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://wvz.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://awj.aizwys.cn

[S03] C：读入整数
来源：http://lyj.bjfxy.top

int x; scanf("%d", &x);
来源：http://hye.snrcjt.cn

[S04] C：字符串复制
来源：http://vtd.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://pkv.sufxvd.cn

[S05] C：字符串长度
来源：http://mtx.fktsv.cn

strlen(s)
来源：http://bgz.ivvv.top

[S06] C：字符串比较
来源：http://dxs.iojbl.cn

strcmp(a, b) == 0
来源：http://aic.dashuyun.cn

[S07] C：数组遍历求和
来源：http://ept.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qjm.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://nrj.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://olj.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://sfx.shanyushiyangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sqv.c1oappe.top

[S10] C：指针与解引用
来源：http://yid.birdmap.top

int *p = &a;  *p = 5;
来源：http://kso.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://qro.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://qso.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://svz.yuanzhike.top

fclose(f);
来源：http://nrx.andypj.xyz

[S12] C：写文件
来源：http://ykt.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qcq.yj20258.top

[S13] C：宏定义
来源：http://wwb.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jrh.fzhhl.top

[S14] C：枚举
来源：http://dia.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://jcz.jyoumei.cn

[S15] C：类型转换
来源：http://ugo.guannengcc.top

(double) a / b
来源：http://zxu.smart0.xyz

[S16] C：位操作置位
来源：http://juo.nwbrower.top

x |= (1 << 3);
来源：http://bzj.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://xev.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qub.fengsongda.top

[S18] C：命令行参数
来源：http://res.nanxuanxn.top

int main(int argc, char **argv)
来源：http://jyo.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://vro.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zcu.feifeiyinyue.top

[S20] C：二分查找
来源：http://frc.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ajk.yuxming.cn

[S21] C：字符类别判断
来源：http://izu.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cns.nanxinkj.top

[S22] C：字符串转数字
来源：http://pko.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://scu.hysaishi.cn

[S23] C：随机数
来源：http://gez.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vlg.quarkkingdee.top

[S24] C：获取本地时间
来源：http://mro.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xoy.shzxlz.cn

[S25] C：内存拷贝
来源：http://hmn.yanxiufei.cn

memcpy(dst, src, n);
来源：http://dlh.hnxiangtu.top

[S26] C：内存清零
来源：http://hhw.gzhubu.top

memset(a, 0, sizeof a);
来源：http://pbn.jiagoushi.top

[S27] C：定义常量
来源：http://cxo.shangyingyoupin.top

const double PI = 3.14159;
来源：http://njf.jyoumei.cn

[S28] C：静态变量
来源：http://qmc.gaohongyu789.top

static int counter = 0;
来源：http://szb.xziqi.cn

[S29] C：变参函数
来源：http://oik.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wyq.chenjidiqi.icu

[S30] C：头文件保护
来源：http://yeh.fanxiaobao.xyz

#ifndef X_H
来源：http://njs.daxiang520.top

#define X_H
来源：http://xty.quarkkingdee.top

#endif
来源：http://iss.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://uml.ywan-chungtsiang.top

#include <iostream>
来源：http://hsn.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://uhi.nanxinkj.top

[S32] C++：字符串
来源：http://vud.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://tdc.hysaishi.cn

[S33] C++：vector 增删
来源：http://leb.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vmh.haohaochexian.top

[S34] C++：遍历 vector
来源：http://eht.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://iaw.bbcook.cn

[S35] C++：map
来源：http://oab.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lgt.fzhhl.top

[S36] C++：unordered_map
来源：http://slp.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dpv.ybcxt.top

[S37] C++：set
来源：http://ypa.hysaishi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fhm.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://qez.xinyue.icu

std::sort(v.begin(), v.end());
来源：http://wmg.hesvh.cn


<!-- 参考信息 -->