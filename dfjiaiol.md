代发 wailian999

[Q76] 按天统计
来源：http://yao.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://udm.ppjwa.cn

[Q77] 时间加减
来源：http://tgy.shanyushiyangtech.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gig.sufxvd.cn

[Q78] 当前时间
来源：http://kvq.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vjs.c1oappe.top

[Q79] 字符串拼接
来源：http://mza.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mrd.yonumen.top

[Q80] 字符串截取
来源：http://pgn.yonumen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wnn.kuanghao11.cn

[Q81] 字符串替换
来源：http://ztb.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kdg.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://yth.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mbd.cheryme.top

[Q83] 大小写转换
来源：http://fjb.andypj.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tik.cdnleiting.top

[Q84] 去除首尾空格
来源：http://hca.iojbl.cn

SELECT TRIM(name) FROM users;
来源：http://qij.jianghu66.top

[Q85] 数值取整
来源：http://tvw.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gyu.zhongyouzk.top

[Q86] 读取 JSON 字段
来源：http://aro.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xor.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://ups.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jyg.jinqigufen.top

[Q88] 行转列（条件聚合）
来源：http://buu.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ptv.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oxg.smart0.xyz

[Q89] 判断表是否存在
来源：http://suu.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vur.hesvh.cn

[Q90] 生成序号列
来源：http://fvm.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cjh.daxiang520.top

================================================================================
来源：http://sxc.cucudq.cn

R. Bash 专题
来源：http://koy.zhongyouzk.top

================================================================================
来源：http://smj.fengsongda.top

[R01] shebang 与严格模式
来源：http://prp.yueranfly.top

#!/usr/bin/env bash
来源：http://idi.c1oappe.top

set -euo pipefail
来源：http://ehe.yonumen.top

[R02] 变量赋值与使用
来源：http://dof.tarul.cn

name="Tom"; echo "$name"
来源：http://pxo.aibaodan.cn

[R03] 只读变量
来源：http://ynf.jqgfzy.top

readonly PI=3.14
来源：http://mqi.yvedp.cn

[R04] 位置参数
来源：http://hcx.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ooq.jyoumei.cn

[R05] 参数默认值
来源：http://tni.gaohongyu789.top

name="${1:-default}"
来源：http://ddz.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://cmq.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qno.redwolf501.top

[R07] if 判断文件
来源：http://gms.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ffn.hywenlv.cn

[R08] 数值比较
来源：http://rrt.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://uow.chenjidiqi.icu

[R09] 字符串比较
来源：http://qde.haohaochexian.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ljx.smart0.xyz

[R10] 正则匹配
来源：http://gie.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ztv.epnwcf.com

[R11] case 多分支
来源：http://arq.daria6918.cn

case "$1" in
来源：http://fim.yfazqb.com

start) echo "启动" ;;
来源：http://fbn.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://yzg.tian-w.cn

*)     echo "未知命令" ;;
来源：http://umu.redwolf501.top

esac
来源：http://ozl.zdbjq.cn

[R12] for 遍历文件
来源：http://qlk.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://ouc.zdbjq.cn

[R13] for 计数循环
来源：http://tff.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://hrn.vehdjk.com

[R14] C 风格 for
来源：http://xmj.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bii.haohaochexian.top

[R15] while 逐行读文件
来源：http://vij.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ses.tarul.cn

[R16] until 等待条件
来源：http://ecj.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fko.svipenyu.cn

[R17] 数组定义与取值
来源：http://dhz.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kyq.vqdsnc.cn

[R18] 遍历数组
来源：http://wtw.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://udg.yanxiufei.cn

[R19] 数组长度
来源：http://jcv.shzxlz.cn

echo "${#arr[@]}"
来源：http://iaa.zhengqikj.top

[R20] 关联数组（字典）
来源：http://cso.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mkl.0kj1m.cn

[R21] 字符串长度
来源：http://ccw.pycfn.com

echo "${#s}"
来源：http://gsk.ydzc1.top

[R22] 截取子串
来源：http://njg.sjlbkw.cn

echo "${s:0:5}"
来源：http://cgm.jlsjyb.cn

[R23] 字符串替换
来源：http://sgs.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ozp.yanxiufei.cn

[R24] 大小写转换
来源：http://guu.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://hqr.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://teu.xylfe.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://row.gogol.net.cn

[R26] 命令替换
来源：http://mpq.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://hqt.tianlin.xyz

[R27] 算术展开
来源：http://neu.uphjek.com

echo $((1 + 2 * 3))
来源：http://lmd.jinqigufen.top

[R28] 浮点运算
来源：http://ufa.xinyue.icu

echo "scale=2; 10/3" | bc
来源：http://sxv.gogol.net.cn

[R29] 定义函数
来源：http://vcd.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lfl.316326.xyz

[R30] 函数返回状态码
来源：http://dnb.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://yeu.hcnkem.com

[R31] 局部变量
来源：http://ouv.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://cpu.kuanghao11.cn

[R32] 参数个数校验
来源：http://bid.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lhg.tarul.cn

[R33] 捕获错误并提示行号
来源：http://vul.fengsongda.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vly.ybcxt.top

[R34] 退出时清理
来源：http://jbc.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://rli.gogol.net.cn

[R35] 后台执行并等待
来源：http://har.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wtk.tianlin.xyz

[R36] 并发执行多个任务
来源：http://pjy.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mpr.cashguo.top

[R37] 把输出赋给变量
来源：http://vdp.jinyuanbaomall.cn

files=$(ls -1)
来源：http://mex.meibo888.top

[R38] 管道串联
来源：http://bgm.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://vhl.zhixingplan.top

[R39] 重定向标准输出与错误
来源：http://fhh.yfazqb.com

cmd > out.log 2>&1
来源：http://rnq.cqqwz.cn

[R40] 追加写日志
来源：http://xgj.vehdjk.com

echo "log" >> out.log
来源：http://pov.jinqigfzy.top

[R41] 丢弃输出
来源：http://fja.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://ycl.zdqjudy.top

[R42] 输入重定向
来源：http://uxv.zhiwuduotai.top

wc -l < a.txt
来源：http://qep.9152youxi.cn

[R43] 按名字查找文件
来源：http://jmi.shzxlz.cn

find . -name "*.log" -type f
来源：http://mao.xinyue.icu

[R44] 按修改时间查找
来源：http://muy.yonumen.top

find . -mtime -7 -type f
来源：http://inq.yangfankeji.com

[R45] 批量删除
来源：http://qht.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://uyj.cashguo.top

[R46] 递归替换文件内容
来源：http://nos.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jfl.fengsongda.top

[R47] sed 单行替换
来源：http://evx.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ctz.zdqjudy.top

[R48] awk 取指定列
来源：http://xrw.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://zqb.quarkkingdee.top

[R49] awk 带条件
来源：http://qam.shanyushiyangtech.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://goa.jyoumei.cn

[R50] awk 求和
来源：http://cyw.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://ozn.fzhhl.top

[R51] 排序去重取前几
来源：http://uts.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://epb.xinyue.icu

[R52] 统计行数
来源：http://aag.tianlin.xyz

wc -l a.txt
来源：http://vve.cashguo.top

[R53] 查看文件头与实时尾
来源：http://vba.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hpg.zhoulong.xyz

[R54] 比较两个文件
来源：http://yfu.hammf.cn

diff a.txt b.txt
来源：http://hck.zhijiandao.cn

[R55] 压缩与解压
来源：http://jcp.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cwb.tarul.cn

[R56] 远程拷贝
来源：http://wfi.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://yue.fktsv.cn

[R57] 远程执行命令
来源：http://fhu.aibaodan.cn

ssh user@host 'uptime'
来源：http://zem.zhixingplan.top

[R58] 下载文件
来源：http://hml.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oru.ehwqpu.com

[R59] 发 POST JSON
来源：http://lfx.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xcp.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://vbd.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jst.jqgfzy.top

[R61] 磁盘占用
来源：http://asi.birdmap.top

df -h;  du -sh *
来源：http://qae.dianchejie.cn

[R62] 找最占空间的文件
来源：http://wtn.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://vwv.yvedp.cn

[R63] 内存与进程
来源：http://cvh.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://avh.ehwqpu.com

[R64] 结束进程
来源：http://ycf.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://hes.yangfankeji.com

[R65] 查看端口占用
来源：http://sxf.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jcr.havefunace.top

[R66] 定时任务
来源：http://xjl.tanke756.top

crontab -e;  crontab -l
来源：http://fes.fktsv.cn

[R67] 生成随机十六进制串
来源：http://xrg.havefunace.top

openssl rand -hex 16
来源：http://elv.chenlongwang.top

[R68] 计算文件校验值
来源：http://bgt.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://khu.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://onh.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://rlg.zhoulong.xyz

[R70] 时间戳与互转
来源：http://twk.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://rkm.jianghu66.top

[R71] 日期格式化
来源：http://gge.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ywj.cqqwz.cn

[R72] 等待端口就绪
来源：http://tnt.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wkg.nwbrower.top

[R73] 分割大日志
来源：http://fnc.pycfn.com

split -l 1000 big.log part_
来源：http://hel.fanxiaobao.xyz

[R74] 批量重命名
来源：http://oyl.zhengqikj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fve.xylfe.cn

[R75] 导出环境变量
来源：http://oki.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://llb.daxiang520.top

[R76] 使用临时文件
来源：http://bze.quarkkingdee.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xzs.shzxlz.cn

[R77] 读取用户输入
来源：http://adt.gotoacloud.top

read -rp "请输入: " ans
来源：http://nwo.gotoacloud.top

[R78] 交互式菜单
来源：http://jvx.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://pki.redwolf501.top

[R79] 解析命令行选项
来源：http://eer.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baw.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://lvf.hongshengwenyu.top

time ./run.sh
来源：http://hiu.0kj1m.cn

================================================================================
来源：http://xxc.gotoacloud.top

S. C / C++ 专题
来源：http://lgk.zhengqikj.top

================================================================================
来源：http://rkl.sjlbkw.cn

[S01] C：Hello World
来源：http://pmh.52xcode.cn

#include <stdio.h>
来源：http://vsc.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oxq.sweek.top

[S02] C：变量与格式化输出
来源：http://tun.haohaochexian.top

int a = 10; printf("%d\n", a);
来源：http://rbm.quarkkingdee.top

[S03] C：读入整数
来源：http://syt.redwolf501.top

int x; scanf("%d", &x);
来源：http://dqv.cucudq.cn

[S04] C：字符串复制
来源：http://hsw.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nsc.fzhhl.top

[S05] C：字符串长度
来源：http://txg.pengpengdd.cyou

strlen(s)
来源：http://yxs.jinqigfzy.top

[S06] C：字符串比较
来源：http://iku.316326.xyz

strcmp(a, b) == 0
来源：http://abn.zhixingplan.top

[S07] C：数组遍历求和
来源：http://lek.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vig.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://ezp.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nkx.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://shu.tian-w.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bkp.yanxiufei.cn

[S10] C：指针与解引用
来源：http://oiq.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://osv.svipenyu.cn

[S11] C：逐行读文件
来源：http://qnw.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://jbg.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://eci.yanxiufei.cn

fclose(f);
来源：http://mov.c1oappe.top

[S12] C：写文件
来源：http://zfn.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ufp.sysykeji.top

[S13] C：宏定义
来源：http://kfl.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nkj.daria6918.cn

[S14] C：枚举
来源：http://kkk.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://raq.havefunace.top

[S15] C：类型转换
来源：http://wjj.yonumen.top

(double) a / b
来源：http://eoa.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://gtx.redwolf501.top

x |= (1 << 3);
来源：http://vxf.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://gih.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bwb.ehwqpu.com

[S18] C：命令行参数
来源：http://abn.jyoumei.cn

int main(int argc, char **argv)
来源：http://jby.hongshengwenyu.top

[S19] C：快速排序
来源：http://fou.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://str.andypj.xyz

[S20] C：二分查找
来源：http://buq.jianghu66.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://atw.yanxiufei.cn

[S21] C：字符类别判断
来源：http://qds.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qtq.xinyue.icu

[S22] C：字符串转数字
来源：http://mrq.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://omp.dianchejie.cn

[S23] C：随机数
来源：http://ncq.cucudq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ohp.hywenlv.cn

[S24] C：获取本地时间
来源：http://iea.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dnz.yanxiufei.cn

[S25] C：内存拷贝
来源：http://fyf.guannengcc.top

memcpy(dst, src, n);
来源：http://gxn.shuidangran.top

[S26] C：内存清零
来源：http://ckk.sysykeji.top

memset(a, 0, sizeof a);
来源：http://gsj.tanke756.top

[S27] C：定义常量
来源：http://pot.cheryme.top

const double PI = 3.14159;
来源：http://ely.gzhubu.top

[S28] C：静态变量
来源：http://nok.jyoumei.cn

static int counter = 0;
来源：http://psd.hnqzz.top

[S29] C：变参函数
来源：http://fvk.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aql.yuxming.cn

[S30] C：头文件保护
来源：http://zma.hnqzz.top

#ifndef X_H
来源：http://ymt.fanxiaobao.xyz

#define X_H
来源：http://dfh.vehdjk.com

#endif
来源：http://nud.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://pgx.cqqwz.cn

#include <iostream>
来源：http://bez.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://wex.zhongyouzk.top

[S32] C++：字符串
来源：http://pxh.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://imb.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://nul.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qhf.ctjpmb.com

[S34] C++：遍历 vector
来源：http://tnt.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://tkk.yongpay.top

[S35] C++：map
来源：http://uzc.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zxt.cqqwz.cn

[S36] C++：unordered_map
来源：http://dco.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qfc.chenzaomai.com

[S37] C++：set
来源：http://vkk.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://agv.meibo888.top

[S38] C++：排序
来源：http://kfa.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://rdz.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://cko.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iax.snrcjt.cn

[S40] C++：查找元素
来源：http://mbq.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jrk.fktsv.cn

[S41] C++：类与构造函数
来源：http://npr.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bhf.jianghu66.top

[S42] C++：继承与虚函数
来源：http://xdy.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://xkt.nanxinkj.top

[S43] C++：智能指针
来源：http://nxu.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://qqj.cqqwz.cn

[S44] C++：引用传参
来源：http://ajz.zhaomingkeji.xyz

void inc(int &x) { ++x; }
来源：http://izq.sufxvd.cn

[S45] C++：lambda
来源：http://yer.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jyq.ehwqpu.com

[S46] C++：函数模板
来源：http://gkg.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zhz.gotoacloud.top


<!-- 参考信息 -->