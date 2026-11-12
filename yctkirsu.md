代发 wailian999

[Q80] 字符串截取
来源：http://fpn.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kif.sxryk.cn

[Q81] 字符串替换
来源：http://hqm.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vcj.redwolf501.top

[Q82] 字符长度与字节长度
来源：http://pui.iojbl.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qer.hammf.cn

[Q83] 大小写转换
来源：http://btp.fktsv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ocn.xinyue.icu

[Q84] 去除首尾空格
来源：http://yht.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://khb.ydjk.org.cn

[Q85] 数值取整
来源：http://rdg.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zuj.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://mzl.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pxf.sweek.top

[Q87] JSON 字段做条件
来源：http://hjo.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uvz.wangdashe.top

[Q88] 行转列（条件聚合）
来源：http://ybv.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vha.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hag.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://whf.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rba.quarkkingdee.top

[Q90] 生成序号列
来源：http://vqs.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uno.daxiang520.top

================================================================================
来源：http://iaz.xinyue.icu

R. Bash 专题
来源：http://qyj.gogol.net.cn

================================================================================
来源：http://iur.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://crk.ivvv.top

#!/usr/bin/env bash
来源：http://uta.52xcode.cn

set -euo pipefail
来源：http://hmb.svipenyu.cn

[R02] 变量赋值与使用
来源：http://dac.tian-w.cn

name="Tom"; echo "$name"
来源：http://qur.yuxming.cn

[R03] 只读变量
来源：http://pat.xziqi.cn

readonly PI=3.14
来源：http://ypr.tanke756.top

[R04] 位置参数
来源：http://nbw.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tcz.hnqzz.top

[R05] 参数默认值
来源：http://rhe.fengsongda.top

name="${1:-default}"
来源：http://cdb.vehdjk.com

[R06] 判断命令是否存在
来源：http://zua.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ahh.yuxming.cn

[R07] if 判断文件
来源：http://slv.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kou.tianlin.xyz

[R08] 数值比较
来源：http://zvw.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://omn.sjlbkw.cn

[R09] 字符串比较
来源：http://iur.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fjk.zhongyouzk.top

[R10] 正则匹配
来源：http://elt.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ooq.zycfv.cn

[R11] case 多分支
来源：http://rfb.xziqi.cn

case "$1" in
来源：http://lqs.yanxiufei.cn

start) echo "启动" ;;
来源：http://ufx.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://gwx.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://zwi.zhongyouzk.top

esac
来源：http://lzl.xylfe.cn

[R12] for 遍历文件
来源：http://iwr.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://rwx.haohaochexian.top

[R13] for 计数循环
来源：http://dvw.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://kjh.guannengcc.top

[R14] C 风格 for
来源：http://pgs.yangfankeji.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yuy.vqdsnc.cn

[R15] while 逐行读文件
来源：http://uad.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qah.fengsongda.top

[R16] until 等待条件
来源：http://xyf.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cns.tianlin.xyz

[R17] 数组定义与取值
来源：http://bcw.fengsongda.top

arr=(a b c); echo "${arr[0]}"
来源：http://yao.havefunace.top

[R18] 遍历数组
来源：http://dmo.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dwb.zhiwuduotai.top

[R19] 数组长度
来源：http://vmo.52xcode.cn

echo "${#arr[@]}"
来源：http://gtf.zhengqikj.top

[R20] 关联数组（字典）
来源：http://sux.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fwq.hywenlv.cn

[R21] 字符串长度
来源：http://nid.zhixingplan.top

echo "${#s}"
来源：http://raw.hesvh.cn

[R22] 截取子串
来源：http://xkv.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://jee.guannengcc.top

[R23] 字符串替换
来源：http://ewv.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dxn.hywenlv.cn

[R24] 大小写转换
来源：http://ktd.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://geu.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://iwe.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vqk.sweek.top

[R26] 命令替换
来源：http://ynp.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://tiy.jianghu66.top

[R27] 算术展开
来源：http://ggm.fzhhl.top

echo $((1 + 2 * 3))
来源：http://sit.pycfn.com

[R28] 浮点运算
来源：http://zlc.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://pvl.gzhubu.top

[R29] 定义函数
来源：http://ihj.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vag.yfazqb.com

[R30] 函数返回状态码
来源：http://rml.jlsjyb.cn

f() { return 0; }; f || echo "失败了"
来源：http://lzb.vehdjk.com

[R31] 局部变量
来源：http://ltj.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://dyc.meibo888.top

[R32] 参数个数校验
来源：http://qwy.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lzk.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://khi.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mov.yj20258888.top

[R34] 退出时清理
来源：http://xhj.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rzi.yangfankeji.com

[R35] 后台执行并等待
来源：http://edw.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wmq.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://nwn.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jga.cheryme.top

[R37] 把输出赋给变量
来源：http://ywr.xuanzx.com

files=$(ls -1)
来源：http://yxm.ctjpmb.com

[R38] 管道串联
来源：http://kyu.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://kxq.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://pjx.cucudq.cn

cmd > out.log 2>&1
来源：http://zxh.gotoacloud.top

[R40] 追加写日志
来源：http://tkd.zhongyouzk.top

echo "log" >> out.log
来源：http://blq.meibo888.top

[R41] 丢弃输出
来源：http://knh.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://wxi.yangfankeji.com

[R42] 输入重定向
来源：http://znf.ybcxt.top

wc -l < a.txt
来源：http://lta.ctjpmb.com

[R43] 按名字查找文件
来源：http://nln.yuanzhike.top

find . -name "*.log" -type f
来源：http://onq.chenlongwang.top

[R44] 按修改时间查找
来源：http://cxy.yonumen.top

find . -mtime -7 -type f
来源：http://gnd.guannengcc.top

[R45] 批量删除
来源：http://qss.zycfv.cn

find . -name "*.tmp" -delete
来源：http://zji.fzhhl.top

[R46] 递归替换文件内容
来源：http://uiu.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dbk.52xcode.cn

[R47] sed 单行替换
来源：http://scj.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zmw.yj20258.top

[R48] awk 取指定列
来源：http://jkj.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://rqx.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://lri.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ajr.zhengqikj.top

[R50] awk 求和
来源：http://ued.zhaomingkeji.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://wmk.dashuyun.cn

[R51] 排序去重取前几
来源：http://lot.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://blt.xuanzx.com

[R52] 统计行数
来源：http://oqi.zhixingplan.top

wc -l a.txt
来源：http://wgz.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://itp.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://grv.havefunace.top

[R54] 比较两个文件
来源：http://vsh.vehdjk.com

diff a.txt b.txt
来源：http://mdg.mhx1999.top

[R55] 压缩与解压
来源：http://upb.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sxz.jianghu66.top

[R56] 远程拷贝
来源：http://tko.chenzaomai.com

scp file user@host:/path/
来源：http://wed.gotoacloud.top

[R57] 远程执行命令
来源：http://gha.svipenyu.cn

ssh user@host 'uptime'
来源：http://hgr.chenzaomai.com

[R58] 下载文件
来源：http://jfg.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vud.guowangkeji.top

[R59] 发 POST JSON
来源：http://wvd.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dfk.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://voh.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cra.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://udy.hongshengwenyu.top

df -h;  du -sh *
来源：http://pxy.fehbvm.com

[R62] 找最占空间的文件
来源：http://qkj.tanke756.top

du -ah . | sort -rh | head -10
来源：http://kus.jiagoushi.top

[R63] 内存与进程
来源：http://ccy.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://hmw.xuanzx.com

[R64] 结束进程
来源：http://uza.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://juh.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://nmd.jlsjyb.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wwm.zycfv.cn

[R66] 定时任务
来源：http://xxy.9152youxi.cn

crontab -e;  crontab -l
来源：http://yfv.fehbvm.com

[R67] 生成随机十六进制串
来源：http://viu.guowangkeji.top

openssl rand -hex 16
来源：http://nkt.ydjk.org.cn

[R68] 计算文件校验值
来源：http://cwp.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xeu.hammf.cn

[R69] 生成随机密码
来源：http://ozz.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://hgc.hammf.cn

[R70] 时间戳与互转
来源：http://ile.yj20258.top

date +%s;  date -d @1700000000
来源：http://llb.fktsv.cn

[R71] 日期格式化
来源：http://dyl.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pjw.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://vdc.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wfm.jqgfzy.top

[R73] 分割大日志
来源：http://lwl.haohaochexian.top

split -l 1000 big.log part_
来源：http://qgu.xuanzx.com

[R74] 批量重命名
来源：http://kiv.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yww.uphjek.com

[R75] 导出环境变量
来源：http://urb.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://fpm.zhengqikj.top

[R76] 使用临时文件
来源：http://sog.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yfs.zhengqikj.top

[R77] 读取用户输入
来源：http://dou.cdnleiting.top

read -rp "请输入: " ans
来源：http://wxu.zhoulong.xyz

[R78] 交互式菜单
来源：http://xtj.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://unn.yj20258.top

[R79] 解析命令行选项
来源：http://yxn.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hhw.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://qca.jianghu66.top

time ./run.sh
来源：http://pio.svipenyu.cn

================================================================================
来源：http://omr.jiagoushi.top

S. C / C++ 专题
来源：http://dht.vqdsnc.cn

================================================================================
来源：http://frx.yonumen.top

[S01] C：Hello World
来源：http://roh.ctjpmb.com

#include <stdio.h>
来源：http://nxv.nanxinkj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gsz.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://wef.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://ifp.jinqigufen.top

[S03] C：读入整数
来源：http://dnw.shzxlz.cn

int x; scanf("%d", &x);
来源：http://kff.hesvh.cn

[S04] C：字符串复制
来源：http://dhb.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ubk.zhengqikj.top

[S05] C：字符串长度
来源：http://qnp.smart0.xyz

strlen(s)
来源：http://bqg.ivvv.top

[S06] C：字符串比较
来源：http://frj.pycfn.com

strcmp(a, b) == 0
来源：http://gtj.daria6918.cn

[S07] C：数组遍历求和
来源：http://nda.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hzk.jqgfzy.top

[S08] C：动态内存分配与释放
来源：http://inm.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ahi.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://ofg.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mzv.aibaodan.cn

[S10] C：指针与解引用
来源：http://fvz.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://tba.cqqwz.cn

[S11] C：逐行读文件
来源：http://atz.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://wsv.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xmw.vqdsnc.cn

fclose(f);
来源：http://qks.tarul.cn

[S12] C：写文件
来源：http://chx.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ozq.cashguo.top

[S13] C：宏定义
来源：http://pzu.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pqq.snrcjt.cn

[S14] C：枚举
来源：http://aug.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://vee.jinqigfzy.top

[S15] C：类型转换
来源：http://wor.hnqzz.top

(double) a / b
来源：http://nua.ehwqpu.com

[S16] C：位操作置位
来源：http://pda.chenzaomai.com

x |= (1 << 3);
来源：http://rqr.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://iuw.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ede.vehdjk.com

[S18] C：命令行参数
来源：http://ywu.xziqi.cn

int main(int argc, char **argv)
来源：http://lqv.dashuyun.cn

[S19] C：快速排序
来源：http://qhu.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://qac.jinqigfzy.top

[S20] C：二分查找
来源：http://wcp.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xyu.xylfe.cn

[S21] C：字符类别判断
来源：http://maa.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iuv.redwolf501.top

[S22] C：字符串转数字
来源：http://ykt.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://euj.redwolf501.top

[S23] C：随机数
来源：http://olq.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fgr.9152youxi.cn

[S24] C：获取本地时间
来源：http://ejk.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://auh.jlsjyb.cn

[S25] C：内存拷贝
来源：http://jqu.guannengcc.top

memcpy(dst, src, n);
来源：http://ihj.cqqwz.cn

[S26] C：内存清零
来源：http://vav.cdnleiting.top

memset(a, 0, sizeof a);
来源：http://mzs.hnxiangtu.top

[S27] C：定义常量
来源：http://fzc.pengpengdd.cyou

const double PI = 3.14159;
来源：http://kms.dashuyun.cn

[S28] C：静态变量
来源：http://eew.52xcode.cn

static int counter = 0;
来源：http://xti.ivvv.top

[S29] C：变参函数
来源：http://lhm.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://coc.nanxuanxn.top

[S30] C：头文件保护
来源：http://vji.jinqigfzy.top

#ifndef X_H
来源：http://gej.tanke756.top

#define X_H
来源：http://sca.ehwqpu.com

#endif
来源：http://wii.guannengcc.top

[S31] C++：Hello World
来源：http://mbj.jiagoushi.top

#include <iostream>
来源：http://vmo.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://zvr.havefunace.top

[S32] C++：字符串
来源：http://tcs.shanyushiyangtech.top

std::string s = "hi";  s += "!";
来源：http://ivs.yuxming.cn

[S33] C++：vector 增删
来源：http://gzj.svipenyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dep.hammf.cn

[S34] C++：遍历 vector
来源：http://hyk.dashuyun.cn

for (auto &x : v) { std::cout << x; }
来源：http://tuf.havefunace.top

[S35] C++：map
来源：http://qxl.daria6918.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rpc.fehbvm.com

[S36] C++：unordered_map
来源：http://tbp.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rpv.pengpengdd.cyou

[S37] C++：set
来源：http://rwf.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pch.xylfe.cn

[S38] C++：排序
来源：http://ewq.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://tww.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://ukq.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aqo.zhengqikj.top

[S40] C++：查找元素
来源：http://ygr.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://abg.316326.xyz

[S41] C++：类与构造函数
来源：http://gex.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cer.bbcook.cn

[S42] C++：继承与虚函数
来源：http://nep.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://jvf.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://uth.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://usr.nanxinkj.top

[S44] C++：引用传参
来源：http://qfg.fktsv.cn

void inc(int &x) { ++x; }
来源：http://kcm.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://mhr.jinqigfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://rxs.guannengcc.top

[S46] C++：函数模板
来源：http://dkd.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lcb.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://zfc.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nvx.hnxiangtu.top

[S48] C++：逐行读文件
来源：http://foy.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://azt.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://pyt.jinghuilouyu.cn

[S49] C++：写文件
来源：http://wkv.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xtr.pycfn.com

[S50] C++：格式化数字
来源：http://lpy.yj20258.top


<!-- 参考信息 -->