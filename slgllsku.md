代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pjx.haohaochexian.top

[Q75] 日期格式化
来源：http://cls.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ryu.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vsj.zhiwuduotai.top

[Q76] 按天统计
来源：http://vnx.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fxa.vehdjk.com

[Q77] 时间加减
来源：http://juf.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lij.aizwys.cn

[Q78] 当前时间
来源：http://hvw.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://srt.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://tjd.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tzm.ppjwa.cn

[Q80] 字符串截取
来源：http://qmb.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fyy.hcnkem.com

[Q81] 字符串替换
来源：http://bmb.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iuy.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://qdc.meibo888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hfp.cucudq.cn

[Q83] 大小写转换
来源：http://gwl.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xdm.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://cou.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://xbf.cucudq.cn

[Q85] 数值取整
来源：http://xko.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ewt.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://dvk.ctjpmb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oby.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://zet.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jps.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://eqo.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oey.jyoumei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tqw.9152youxi.cn

[Q89] 判断表是否存在
来源：http://dnp.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://prh.tian-w.cn

[Q90] 生成序号列
来源：http://xdx.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jus.nanxinkj.top

================================================================================
来源：http://wdl.birdmap.top

R. Bash 专题
来源：http://zhy.gogol.net.cn

================================================================================
来源：http://btv.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://kbu.vehdjk.com

#!/usr/bin/env bash
来源：http://qkq.hnqzz.top

set -euo pipefail
来源：http://enh.hammf.cn

[R02] 变量赋值与使用
来源：http://tal.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://cuu.jlsjyb.cn

[R03] 只读变量
来源：http://nbt.ydjk.org.cn

readonly PI=3.14
来源：http://nkm.hcnkem.com

[R04] 位置参数
来源：http://pek.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xhq.cucudq.cn

[R05] 参数默认值
来源：http://qmv.hnqzz.top

name="${1:-default}"
来源：http://fqt.hfpthk.cn

[R06] 判断命令是否存在
来源：http://kdo.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eie.haohaochexian.top

[R07] if 判断文件
来源：http://jlm.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ods.jinyuanbaomall.cn

[R08] 数值比较
来源：http://lom.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rum.smart0.xyz

[R09] 字符串比较
来源：http://orw.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://seq.ppjwa.cn

[R10] 正则匹配
来源：http://mwf.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fny.wangdashe.top

[R11] case 多分支
来源：http://pjv.yongpay.top

case "$1" in
来源：http://tff.yangfankeji.com

start) echo "启动" ;;
来源：http://frf.aizwys.cn

stop)  echo "停止" ;;
来源：http://meq.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://zsx.guannengcc.top

esac
来源：http://ecs.zdbjq.cn

[R12] for 遍历文件
来源：http://kqp.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://kuw.dianchejie.cn

[R13] for 计数循环
来源：http://rrf.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://niq.uphjek.com

[R14] C 风格 for
来源：http://tew.fzhhl.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vjy.yanxiufei.cn

[R15] while 逐行读文件
来源：http://kvs.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tta.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://jwq.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nla.uphjek.com

[R17] 数组定义与取值
来源：http://cav.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://qtm.cashguo.top

[R18] 遍历数组
来源：http://guv.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gme.shanyushiyangtech.top

[R19] 数组长度
来源：http://ofy.chenzaomai.com

echo "${#arr[@]}"
来源：http://pmy.uphjek.com

[R20] 关联数组（字典）
来源：http://vti.shzxlz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://prf.fengsongda.top

[R21] 字符串长度
来源：http://mni.yj20258888.top

echo "${#s}"
来源：http://spr.zhaomingkeji.xyz

[R22] 截取子串
来源：http://yed.jyoumei.cn

echo "${s:0:5}"
来源：http://lhp.ctjpmb.com

[R23] 字符串替换
来源：http://lyv.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rqs.guowangkeji.top

[R24] 大小写转换
来源：http://dxy.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ybf.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://scc.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://agd.yueranfly.top

[R26] 命令替换
来源：http://wnn.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://vde.52xcode.cn

[R27] 算术展开
来源：http://qdw.yonumen.top

echo $((1 + 2 * 3))
来源：http://mby.yangfankeji.com

[R28] 浮点运算
来源：http://fzd.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://xlx.hcnkem.com

[R29] 定义函数
来源：http://jhm.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vbn.jqgfzy.top

[R30] 函数返回状态码
来源：http://jdf.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://igj.ydzc1.top

[R31] 局部变量
来源：http://qic.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://cnz.iojbl.cn

[R32] 参数个数校验
来源：http://iow.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ssb.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://elr.zhaomingkeji.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zrv.zhijiandao.cn

[R34] 退出时清理
来源：http://hjm.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://zem.zhengqikj.top

[R35] 后台执行并等待
来源：http://biw.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qcw.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://gdu.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ykx.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://gin.xylfe.cn

files=$(ls -1)
来源：http://stb.epnwcf.com

[R38] 管道串联
来源：http://htj.yuanzhike.top

cat a.txt | grep -i error | wc -l
来源：http://rlk.guannengcc.top

[R39] 重定向标准输出与错误
来源：http://gbg.iojbl.cn

cmd > out.log 2>&1
来源：http://tdh.tianlin.xyz

[R40] 追加写日志
来源：http://dww.aibaodan.cn

echo "log" >> out.log
来源：http://ids.tianlin.xyz

[R41] 丢弃输出
来源：http://sfm.sweek.top

cmd >/dev/null 2>&1
来源：http://bkt.redwolf501.top

[R42] 输入重定向
来源：http://ufm.jinyuanbaomall.cn

wc -l < a.txt
来源：http://utl.316326.xyz

[R43] 按名字查找文件
来源：http://mjy.yueranfly.top

find . -name "*.log" -type f
来源：http://bfy.jqgufenzy.top

[R44] 按修改时间查找
来源：http://kae.zdbjq.cn

find . -mtime -7 -type f
来源：http://fcs.0kj1m.cn

[R45] 批量删除
来源：http://yze.bbcook.cn

find . -name "*.tmp" -delete
来源：http://jmf.jqgfzy.top

[R46] 递归替换文件内容
来源：http://mql.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://udt.pycfn.com

[R47] sed 单行替换
来源：http://tdn.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://ley.xingfuxueyuan.xyz

[R48] awk 取指定列
来源：http://dmq.sweek.top

awk '{print $1, $3}' a.txt
来源：http://rmr.gotoacloud.top

[R49] awk 带条件
来源：http://vlh.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fvh.svipenyu.cn

[R50] awk 求和
来源：http://jya.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://cxq.hcnkem.com

[R51] 排序去重取前几
来源：http://ifm.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xnf.c1oappe.top

[R52] 统计行数
来源：http://fbh.quarkkingdee.top

wc -l a.txt
来源：http://maw.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://ggx.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bwx.xziqi.cn

[R54] 比较两个文件
来源：http://ezz.tianlin.xyz

diff a.txt b.txt
来源：http://nao.0kj1m.cn

[R55] 压缩与解压
来源：http://tan.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ggl.hnxiangtu.top

[R56] 远程拷贝
来源：http://jea.sysykeji.top

scp file user@host:/path/
来源：http://hgr.hongshengwenyu.top

[R57] 远程执行命令
来源：http://gze.vehdjk.com

ssh user@host 'uptime'
来源：http://oen.yj20258888.top

[R58] 下载文件
来源：http://dmw.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cqt.jinqigfzy.top

[R59] 发 POST JSON
来源：http://fkh.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fbi.chenlongwang.top

[R60] 只看 HTTP 状态码
来源：http://rjc.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jrz.wangshuangyany.cn

[R61] 磁盘占用
来源：http://aqp.zhijiandao.cn

df -h;  du -sh *
来源：http://mmq.sufxvd.cn

[R62] 找最占空间的文件
来源：http://ujg.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://qmr.sysykeji.top

[R63] 内存与进程
来源：http://ysg.epnwcf.com

free -h;  ps aux | grep nginx
来源：http://tdt.zdqjudy.top

[R64] 结束进程
来源：http://sjr.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://nws.zhijiandao.cn

[R65] 查看端口占用
来源：http://ick.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mrh.hfpthk.cn

[R66] 定时任务
来源：http://hxd.aizwys.cn

crontab -e;  crontab -l
来源：http://qay.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://guf.hammf.cn

openssl rand -hex 16
来源：http://egf.zhixingplan.top

[R68] 计算文件校验值
来源：http://ney.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://spu.jlsjyb.cn

[R69] 生成随机密码
来源：http://otd.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://ygw.zhongyouzk.top

[R70] 时间戳与互转
来源：http://hgf.gogol.net.cn

date +%s;  date -d @1700000000
来源：http://kqn.jyoumei.cn

[R71] 日期格式化
来源：http://vrk.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://snj.yj20258.top

[R72] 等待端口就绪
来源：http://fbk.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sec.birdmap.top

[R73] 分割大日志
来源：http://erv.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://mgc.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://dkb.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dtv.zdbjq.cn

[R75] 导出环境变量
来源：http://nhd.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://ckw.tarul.cn

[R76] 使用临时文件
来源：http://cyl.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://twi.zhengqikj.top

[R77] 读取用户输入
来源：http://csa.bbcook.cn

read -rp "请输入: " ans
来源：http://znn.yj202588.top

[R78] 交互式菜单
来源：http://qms.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jlt.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://ulp.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://clq.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://bjn.xylfe.cn

time ./run.sh
来源：http://ttj.9152youxi.cn

================================================================================
来源：http://iux.birdmap.top

S. C / C++ 专题
来源：http://lpz.guowangkeji.top

================================================================================
来源：http://brx.guannengcc.top

[S01] C：Hello World
来源：http://swx.yfazqb.com

#include <stdio.h>
来源：http://mdp.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://mdk.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://tbb.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://fbs.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://lrv.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://jel.cdnleiting.top

[S04] C：字符串复制
来源：http://zix.shanyushiyangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://isz.hammf.cn

[S05] C：字符串长度
来源：http://bzr.hongshengwenyu.top

strlen(s)
来源：http://neb.zhoulong.xyz

[S06] C：字符串比较
来源：http://pav.shuidangran.top

strcmp(a, b) == 0
来源：http://ejp.zycfv.cn

[S07] C：数组遍历求和
来源：http://viw.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://glr.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://xpx.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gqg.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://wdt.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kub.chenzaomai.com

[S10] C：指针与解引用
来源：http://jus.havefunace.top

int *p = &a;  *p = 5;
来源：http://eza.havefunace.top

[S11] C：逐行读文件
来源：http://hrp.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://fzy.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wra.hammf.cn

fclose(f);
来源：http://pso.jinyuanbaomall.cn

[S12] C：写文件
来源：http://ykt.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pqi.cdnleiting.top

[S13] C：宏定义
来源：http://uqt.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://spf.uphjek.com

[S14] C：枚举
来源：http://dec.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://dlr.ppjwa.cn

[S15] C：类型转换
来源：http://zto.jlsjyb.cn

(double) a / b
来源：http://jfg.gaohongyu789.top

[S16] C：位操作置位
来源：http://rhk.xinyue.icu

x |= (1 << 3);
来源：http://nmf.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://izc.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rjf.zhengqikj.top

[S18] C：命令行参数
来源：http://fld.birdmap.top

int main(int argc, char **argv)
来源：http://xlm.jiagoushi.top

[S19] C：快速排序
来源：http://rha.nanxuanxn.top

qsort(a, n, sizeof(int), cmp);
来源：http://kci.316326.xyz

[S20] C：二分查找
来源：http://ssp.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fjs.yongpay.top

[S21] C：字符类别判断
来源：http://iic.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tze.sweek.top

[S22] C：字符串转数字
来源：http://jbp.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ykh.pengpengdd.cyou

[S23] C：随机数
来源：http://fag.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://exb.jinqigufen.top

[S24] C：获取本地时间
来源：http://ztt.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sap.ivvv.top

[S25] C：内存拷贝
来源：http://voc.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://aez.bbcook.cn

[S26] C：内存清零
来源：http://jnp.c1oappe.top

memset(a, 0, sizeof a);
来源：http://rpe.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://mks.zhiwuduotai.top

const double PI = 3.14159;
来源：http://knw.yfazqb.com

[S28] C：静态变量
来源：http://vup.cashguo.top

static int counter = 0;
来源：http://xhh.hongshengwenyu.top

[S29] C：变参函数
来源：http://gbk.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aqq.daria6918.cn

[S30] C：头文件保护
来源：http://dbz.316326.xyz

#ifndef X_H
来源：http://yfk.cdnleiting.top

#define X_H
来源：http://vls.cashguo.top

#endif
来源：http://tsl.jlsjyb.cn

[S31] C++：Hello World
来源：http://lcw.shanyushiyangkeji.top

#include <iostream>
来源：http://xsr.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://ifz.shanyushiyangkeji.top

[S32] C++：字符串
来源：http://pyo.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://dnz.wangdashe.top

[S33] C++：vector 增删
来源：http://oqa.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qga.gogol.net.cn

[S34] C++：遍历 vector
来源：http://lmt.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://jei.sxryk.cn

[S35] C++：map
来源：http://lxf.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mxr.fengsongda.top

[S36] C++：unordered_map
来源：http://puy.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://apm.yj20258888.top

[S37] C++：set
来源：http://kko.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nes.fehbvm.com

[S38] C++：排序
来源：http://cqz.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://tiu.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://ktz.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ffe.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://lrr.sweek.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bvr.ywan-chungtsiang.top

[S41] C++：类与构造函数
来源：http://vue.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://boe.yj20258888.top

[S42] C++：继承与虚函数
来源：http://yxh.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://zrl.hnqzz.top

[S43] C++：智能指针
来源：http://shr.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://hgr.zhijiandao.cn

[S44] C++：引用传参
来源：http://nng.zycfv.cn

void inc(int &x) { ++x; }
来源：http://bid.kuanghao11.cn


<!-- 参考信息 -->