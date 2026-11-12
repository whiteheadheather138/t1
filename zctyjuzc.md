代发 wailian999

[Q78] 当前时间
来源：http://zxx.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://grb.xinyue.icu

[Q79] 字符串拼接
来源：http://rbf.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zoa.yuxming.cn

[Q80] 字符串截取
来源：http://uvg.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wws.ppjwa.cn

[Q81] 字符串替换
来源：http://jql.zhongyouzk.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hcc.iojbl.cn

[Q82] 字符长度与字节长度
来源：http://ycx.yueranfly.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hej.haohaochexian.top

[Q83] 大小写转换
来源：http://tlg.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jov.vqdsnc.cn

[Q84] 去除首尾空格
来源：http://fer.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://hiv.zhiwuduotai.top

[Q85] 数值取整
来源：http://tio.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ssp.316326.xyz

[Q86] 读取 JSON 字段
来源：http://urw.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bwk.iojbl.cn

[Q87] JSON 字段做条件
来源：http://aer.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zsm.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://cdu.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kke.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hrh.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://vui.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vne.yueranfly.top

[Q90] 生成序号列
来源：http://akk.fengsongda.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qdv.ybcxt.top

================================================================================
来源：http://amm.hysaishi.cn

R. Bash 专题
来源：http://fyo.wangdashe.top

================================================================================
来源：http://ipn.hnqzz.top

[R01] shebang 与严格模式
来源：http://jfj.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://cxa.zycfv.cn

set -euo pipefail
来源：http://ubx.yfazqb.com

[R02] 变量赋值与使用
来源：http://kjb.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://kgn.hongshengwenyu.top

[R03] 只读变量
来源：http://euq.jiagoushi.top

readonly PI=3.14
来源：http://tps.jqgufenzy.top

[R04] 位置参数
来源：http://spw.hysaishi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mdn.snrcjt.cn

[R05] 参数默认值
来源：http://zhc.zhengqikj.top

name="${1:-default}"
来源：http://kze.sxryk.cn

[R06] 判断命令是否存在
来源：http://ehc.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ywg.wangdashe.top

[R07] if 判断文件
来源：http://lkl.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qwl.hongshengwenyu.top

[R08] 数值比较
来源：http://gua.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qta.c1oappe.top

[R09] 字符串比较
来源：http://yhc.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dsq.zhoulong.xyz

[R10] 正则匹配
来源：http://hff.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ojt.havefunace.top

[R11] case 多分支
来源：http://pgn.daria6918.cn

case "$1" in
来源：http://fyq.yueranfly.top

start) echo "启动" ;;
来源：http://bpq.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://ryf.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://wcs.mhx1999.top

esac
来源：http://nql.kuanghao11.cn

[R12] for 遍历文件
来源：http://xsz.cucudq.cn

for f in *.txt; do echo "$f"; done
来源：http://dlw.bjfxy.top

[R13] for 计数循环
来源：http://pvw.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://nxo.tanke756.top

[R14] C 风格 for
来源：http://goc.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wat.xuanzx.com

[R15] while 逐行读文件
来源：http://zgv.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://azd.52xcode.cn

[R16] until 等待条件
来源：http://dfm.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yyu.snrcjt.cn

[R17] 数组定义与取值
来源：http://eyy.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pfi.dashuyun.cn

[R18] 遍历数组
来源：http://mtj.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lix.svipenyu.cn

[R19] 数组长度
来源：http://atb.pycfn.com

echo "${#arr[@]}"
来源：http://krr.nwbrower.top

[R20] 关联数组（字典）
来源：http://jog.yanxiufei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eos.havefunace.top

[R21] 字符串长度
来源：http://mdw.xylfe.cn

echo "${#s}"
来源：http://cgz.cdnleiting.top

[R22] 截取子串
来源：http://drd.quarkkingdee.top

echo "${s:0:5}"
来源：http://uaj.snrcjt.cn

[R23] 字符串替换
来源：http://ujo.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mrn.jiagoushi.top

[R24] 大小写转换
来源：http://lsv.ydjk.org.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yhz.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://plw.xylfe.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pyw.ydzc1.top

[R26] 命令替换
来源：http://dep.cdnleiting.top

now=$(date +%F); echo "$now"
来源：http://knp.c1oappe.top

[R27] 算术展开
来源：http://ibu.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://spk.nwbrower.top

[R28] 浮点运算
来源：http://ncd.hesvh.cn

echo "scale=2; 10/3" | bc
来源：http://jzp.wangdashe.top

[R29] 定义函数
来源：http://hvd.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ece.ydzc1.top

[R30] 函数返回状态码
来源：http://qol.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://byt.epnwcf.com

[R31] 局部变量
来源：http://qqg.shanyushiyangtech.top

f() { local x=1; echo "$x"; }
来源：http://qmr.tian-w.cn

[R32] 参数个数校验
来源：http://vct.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sjy.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://twp.ehwqpu.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cne.zhengqikj.top

[R34] 退出时清理
来源：http://byd.chenzaomai.com

trap 'rm -f "$tmp"' EXIT
来源：http://jpy.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://ahs.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rav.hysaishi.cn

[R36] 并发执行多个任务
来源：http://ado.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dvs.hcnkem.com

[R37] 把输出赋给变量
来源：http://cme.zhiwuduotai.top

files=$(ls -1)
来源：http://nqj.jinqigufen.top

[R38] 管道串联
来源：http://vvj.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://qfe.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://aji.hesvh.cn

cmd > out.log 2>&1
来源：http://cof.vehdjk.com

[R40] 追加写日志
来源：http://bsv.tanke756.top

echo "log" >> out.log
来源：http://okw.gotoacloud.top

[R41] 丢弃输出
来源：http://mjj.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://ewu.svipenyu.cn

[R42] 输入重定向
来源：http://lss.tarul.cn

wc -l < a.txt
来源：http://orq.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://dzd.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://fwz.epnwcf.com

[R44] 按修改时间查找
来源：http://cjc.yuanzhike.top

find . -mtime -7 -type f
来源：http://uvx.52xcode.cn

[R45] 批量删除
来源：http://nvr.iojbl.cn

find . -name "*.tmp" -delete
来源：http://ffl.sxryk.cn

[R46] 递归替换文件内容
来源：http://pjy.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rne.bbcook.cn

[R47] sed 单行替换
来源：http://fae.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bmu.jinqigufen.top

[R48] awk 取指定列
来源：http://pbg.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://eyy.jqgufenzy.top

[R49] awk 带条件
来源：http://srx.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qfy.cucudq.cn

[R50] awk 求和
来源：http://ilh.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fym.yonumen.top

[R51] 排序去重取前几
来源：http://vwr.ehwqpu.com

sort a.txt | uniq -c | sort -rn | head
来源：http://gow.snrcjt.cn

[R52] 统计行数
来源：http://hdg.fanxiaobao.xyz

wc -l a.txt
来源：http://hay.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://nfr.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iuc.fehbvm.com

[R54] 比较两个文件
来源：http://xig.zdbjq.cn

diff a.txt b.txt
来源：http://njb.birdmap.top

[R55] 压缩与解压
来源：http://spb.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pkl.zhiwuduotai.top

[R56] 远程拷贝
来源：http://ygl.nanxinkj.top

scp file user@host:/path/
来源：http://zqb.yj20258888.top

[R57] 远程执行命令
来源：http://yxh.cheryme.top

ssh user@host 'uptime'
来源：http://mrc.xinyue.icu

[R58] 下载文件
来源：http://eck.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tvd.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://vzr.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fdg.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://lwy.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wqs.jqgfzy.top

[R61] 磁盘占用
来源：http://kzl.jinqigfzy.top

df -h;  du -sh *
来源：http://amv.hywenlv.cn

[R62] 找最占空间的文件
来源：http://hfn.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://jgz.zhengqikj.top

[R63] 内存与进程
来源：http://bos.havefunace.top

free -h;  ps aux | grep nginx
来源：http://fhm.vqdsnc.cn

[R64] 结束进程
来源：http://ymv.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://qbk.0kj1m.cn

[R65] 查看端口占用
来源：http://obs.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ktk.gzhubu.top

[R66] 定时任务
来源：http://xjj.9152youxi.cn

crontab -e;  crontab -l
来源：http://dll.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://xxo.cdnleiting.top

openssl rand -hex 16
来源：http://uql.vehdjk.com

[R68] 计算文件校验值
来源：http://lia.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://ptg.mhx1999.top

[R69] 生成随机密码
来源：http://mih.gzhubu.top

head -c 16 /dev/urandom | base64
来源：http://rpp.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://ddx.bjfxy.top

date +%s;  date -d @1700000000
来源：http://tql.9152youxi.cn

[R71] 日期格式化
来源：http://jfw.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ehf.hnxiangtu.top

[R72] 等待端口就绪
来源：http://xjp.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://avf.guowangkeji.top

[R73] 分割大日志
来源：http://azm.9152youxi.cn

split -l 1000 big.log part_
来源：http://vkm.dashuyun.cn

[R74] 批量重命名
来源：http://zsv.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nxn.sysykeji.top

[R75] 导出环境变量
来源：http://mbd.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://yfn.ybcxt.top

[R76] 使用临时文件
来源：http://twx.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://exq.316326.xyz

[R77] 读取用户输入
来源：http://xju.yuxming.cn

read -rp "请输入: " ans
来源：http://bdx.hongshengwenyu.top

[R78] 交互式菜单
来源：http://thj.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kva.birdmap.top

[R79] 解析命令行选项
来源：http://xbn.jqgufenzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kqp.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://tws.xylfe.cn

time ./run.sh
来源：http://hwa.dashuyun.cn

================================================================================
来源：http://jmk.chenlongwang.top

S. C / C++ 专题
来源：http://uvz.nanxinkj.top

================================================================================
来源：http://isr.tianlin.xyz

[S01] C：Hello World
来源：http://kua.gzhubu.top

#include <stdio.h>
来源：http://hrh.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ahr.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://nmq.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://tnb.cdnleiting.top

[S03] C：读入整数
来源：http://mtb.jianghu66.top

int x; scanf("%d", &x);
来源：http://xnr.hammf.cn

[S04] C：字符串复制
来源：http://onj.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://gui.jianghu66.top

[S05] C：字符串长度
来源：http://pfb.jianghu66.top

strlen(s)
来源：http://ndu.fehbvm.com

[S06] C：字符串比较
来源：http://spx.zdbjq.cn

strcmp(a, b) == 0
来源：http://fln.smart0.xyz

[S07] C：数组遍历求和
来源：http://lmv.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iur.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://tru.yuxming.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tni.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://nzq.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oan.hcnkem.com

[S10] C：指针与解引用
来源：http://dfg.hnqzz.top

int *p = &a;  *p = 5;
来源：http://bcf.pycfn.com

[S11] C：逐行读文件
来源：http://kzk.yongpay.top

FILE *f = fopen("a.txt", "r");
来源：http://tfv.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qkd.birdmap.top

fclose(f);
来源：http://qad.zhengqikj.top

[S12] C：写文件
来源：http://iby.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xgn.dashuyun.cn

[S13] C：宏定义
来源：http://zrf.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://veh.shangyingyoupin.top

[S14] C：枚举
来源：http://fym.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://rle.316326.xyz

[S15] C：类型转换
来源：http://pqy.ctjpmb.com

(double) a / b
来源：http://brc.fehbvm.com

[S16] C：位操作置位
来源：http://fbw.yongpay.top

x |= (1 << 3);
来源：http://bzg.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://bwz.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hbw.ybcxt.top

[S18] C：命令行参数
来源：http://law.sjlbkw.cn

int main(int argc, char **argv)
来源：http://ymv.yfazqb.com

[S19] C：快速排序
来源：http://oek.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gto.redwolf501.top

[S20] C：二分查找
来源：http://xlj.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zrs.hysaishi.cn

[S21] C：字符类别判断
来源：http://dds.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qts.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://wwb.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://uuo.yj20258.top

[S23] C：随机数
来源：http://qyp.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ykd.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://kki.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zih.tarul.cn

[S25] C：内存拷贝
来源：http://xyi.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://qzr.yuanzhike.top

[S26] C：内存清零
来源：http://yhs.nwbrower.top

memset(a, 0, sizeof a);
来源：http://zya.tian-w.cn

[S27] C：定义常量
来源：http://wzo.fengsongda.top

const double PI = 3.14159;
来源：http://eke.tianlin.xyz

[S28] C：静态变量
来源：http://ruk.guannengcc.top

static int counter = 0;
来源：http://ygt.birdmap.top

[S29] C：变参函数
来源：http://rmp.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vkl.pengpengdd.cyou

[S30] C：头文件保护
来源：http://rtp.zdbjq.cn

#ifndef X_H
来源：http://lho.mhx1999.top

#define X_H
来源：http://dse.quarkkingdee.top

#endif
来源：http://qhf.hnqzz.top

[S31] C++：Hello World
来源：http://xlx.zycfv.cn

#include <iostream>
来源：http://zrm.gzhubu.top

int main() { std::cout << "Hello\n"; }
来源：http://twq.yueranfly.top

[S32] C++：字符串
来源：http://eso.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://sqt.zhengqikj.top

[S33] C++：vector 增删
来源：http://kia.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hrh.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://smt.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://fzj.c1oappe.top

[S35] C++：map
来源：http://fez.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tws.316326.xyz

[S36] C++：unordered_map
来源：http://cbq.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jod.shangyingyoupin.top

[S37] C++：set
来源：http://gzj.pengpengdd.cyou

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qlf.andypj.xyz

[S38] C++：排序
来源：http://wcr.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://apb.havefunace.top

[S39] C++：自定义比较器排序
来源：http://bnt.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eah.yongpay.top

[S40] C++：查找元素
来源：http://eun.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fro.smart0.xyz

[S41] C++：类与构造函数
来源：http://mkj.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://prg.sysykeji.top

[S42] C++：继承与虚函数
来源：http://ops.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://xlv.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://dcj.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://mqn.jianghu66.top

[S44] C++：引用传参
来源：http://soq.bjfxy.top

void inc(int &x) { ++x; }
来源：http://fwv.cucudq.cn

[S45] C++：lambda
来源：http://vfr.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://ozm.jinqigufen.top

[S46] C++：函数模板
来源：http://rwh.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gvq.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://hgz.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dws.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://zeb.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rfd.fengsongda.top


<!-- 参考信息 -->