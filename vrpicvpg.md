代发 wailian999

[Q80] 字符串截取
来源：http://grn.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oio.shzxlz.cn

[Q81] 字符串替换
来源：http://kqq.c1oappe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qzl.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://mie.shzxlz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xko.havefunace.top

[Q83] 大小写转换
来源：http://wtw.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nqi.nwbrower.top

[Q84] 去除首尾空格
来源：http://zdx.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://llb.yuanzhike.top

[Q85] 数值取整
来源：http://ecz.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sef.tanke756.top

[Q86] 读取 JSON 字段
来源：http://zpq.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sib.epnwcf.com

[Q87] JSON 字段做条件
来源：http://msy.shanyushiyangtech.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vcq.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://lra.yvedp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ckd.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kik.sxryk.cn

[Q89] 判断表是否存在
来源：http://mkb.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wyr.gotoacloud.top

[Q90] 生成序号列
来源：http://tzp.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xjl.yuanzhike.top

================================================================================
来源：http://cpf.snrcjt.cn

R. Bash 专题
来源：http://liz.zdqjudy.top

================================================================================
来源：http://vfu.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://ptf.sjlbkw.cn

#!/usr/bin/env bash
来源：http://oxt.zhiwuduotai.top

set -euo pipefail
来源：http://pre.ivvv.top

[R02] 变量赋值与使用
来源：http://kfh.yuanzhike.top

name="Tom"; echo "$name"
来源：http://coi.hesvh.cn

[R03] 只读变量
来源：http://zfo.jinghuilouyu.cn

readonly PI=3.14
来源：http://ydq.ydjk.org.cn

[R04] 位置参数
来源：http://crw.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ydg.yonumen.top

[R05] 参数默认值
来源：http://ubh.chenzaomai.com

name="${1:-default}"
来源：http://gup.mhx1999.top

[R06] 判断命令是否存在
来源：http://tzw.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fte.pycfn.com

[R07] if 判断文件
来源：http://bpe.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mbe.zdqjudy.top

[R08] 数值比较
来源：http://cmt.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dgr.redwolf501.top

[R09] 字符串比较
来源：http://xaz.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gmj.birdmap.top

[R10] 正则匹配
来源：http://dki.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wzr.mhx1999.top

[R11] case 多分支
来源：http://dsx.cqqwz.cn

case "$1" in
来源：http://roe.ydjk.org.cn

start) echo "启动" ;;
来源：http://pqp.hammf.cn

stop)  echo "停止" ;;
来源：http://cfg.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://kim.dashuyun.cn

esac
来源：http://bdd.haohaochexian.top

[R12] for 遍历文件
来源：http://cnw.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://rdr.vqdsnc.cn

[R13] for 计数循环
来源：http://uaq.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://sem.andypj.xyz

[R14] C 风格 for
来源：http://oaj.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wpn.chenzaomai.com

[R15] while 逐行读文件
来源：http://dkb.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pbb.zhijiandao.cn

[R16] until 等待条件
来源：http://kbl.yonumen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lzk.yueranfly.top

[R17] 数组定义与取值
来源：http://gov.yueranfly.top

arr=(a b c); echo "${arr[0]}"
来源：http://ffb.snrcjt.cn

[R18] 遍历数组
来源：http://hnd.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xui.uphjek.com

[R19] 数组长度
来源：http://slk.gogol.net.cn

echo "${#arr[@]}"
来源：http://ric.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://lwu.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ohn.yonumen.top

[R21] 字符串长度
来源：http://wse.aibaodan.cn

echo "${#s}"
来源：http://bko.zycfv.cn

[R22] 截取子串
来源：http://juz.daria6918.cn

echo "${s:0:5}"
来源：http://dmg.yonumen.top

[R23] 字符串替换
来源：http://ajp.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fri.pycfn.com

[R24] 大小写转换
来源：http://gmf.hongshengwenyu.top

echo "${s^^}"; echo "${s,,}"
来源：http://yww.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://vrz.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lsw.aizwys.cn

[R26] 命令替换
来源：http://wmm.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://yql.ivvv.top

[R27] 算术展开
来源：http://qao.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://gxe.9152youxi.cn

[R28] 浮点运算
来源：http://ord.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://paq.sysykeji.top

[R29] 定义函数
来源：http://hsg.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jqd.wangdashe.top

[R30] 函数返回状态码
来源：http://ycx.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://kgb.redwolf501.top

[R31] 局部变量
来源：http://zry.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://zlp.quarkkingdee.top

[R32] 参数个数校验
来源：http://yax.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mko.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://egn.gogol.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://row.aibaodan.cn

[R34] 退出时清理
来源：http://oho.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://iul.fengsongda.top

[R35] 后台执行并等待
来源：http://dpx.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://umz.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://gmf.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://imx.ydzc1.top

[R37] 把输出赋给变量
来源：http://avg.sweek.top

files=$(ls -1)
来源：http://wjt.meibo888.top

[R38] 管道串联
来源：http://nkr.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://zqf.bbcook.cn

[R39] 重定向标准输出与错误
来源：http://ymw.iojbl.cn

cmd > out.log 2>&1
来源：http://upg.bbcook.cn

[R40] 追加写日志
来源：http://jrc.hnqzz.top

echo "log" >> out.log
来源：http://ffh.cqqwz.cn

[R41] 丢弃输出
来源：http://hdx.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://bmt.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://aih.jinyuanbaomall.cn

wc -l < a.txt
来源：http://rfn.yangfankeji.com

[R43] 按名字查找文件
来源：http://wpp.haohaochexian.top

find . -name "*.log" -type f
来源：http://lqe.quarkkingdee.top

[R44] 按修改时间查找
来源：http://vob.jinqigufen.top

find . -mtime -7 -type f
来源：http://yyg.shanyushiyangtech.top

[R45] 批量删除
来源：http://jai.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://cvw.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://yjc.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uuw.sysykeji.top

[R47] sed 单行替换
来源：http://fep.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://pdl.bbcook.cn

[R48] awk 取指定列
来源：http://gtg.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://blv.vehdjk.com

[R49] awk 带条件
来源：http://djc.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://duo.zhongyouzk.top

[R50] awk 求和
来源：http://usm.zdqjudy.top

awk '{s += $2} END {print s}' a.txt
来源：http://tpm.sweek.top

[R51] 排序去重取前几
来源：http://knp.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ptj.cheryme.top

[R52] 统计行数
来源：http://cas.xingfuxueyuan.xyz

wc -l a.txt
来源：http://hxf.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://orq.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vds.tarul.cn

[R54] 比较两个文件
来源：http://ecm.birdmap.top

diff a.txt b.txt
来源：http://czd.wangshuangyany.cn

[R55] 压缩与解压
来源：http://jwf.yongpay.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vza.ehwqpu.com

[R56] 远程拷贝
来源：http://iec.jlsjyb.cn

scp file user@host:/path/
来源：http://ghp.hfpthk.cn

[R57] 远程执行命令
来源：http://xnq.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://dyy.zhijiandao.cn

[R58] 下载文件
来源：http://duj.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kpo.vehdjk.com

[R59] 发 POST JSON
来源：http://qbh.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bod.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://ach.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rjp.hesvh.cn

[R61] 磁盘占用
来源：http://vzc.yueranfly.top

df -h;  du -sh *
来源：http://gba.jinqigufen.top

[R62] 找最占空间的文件
来源：http://xrw.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://lwi.tarul.cn

[R63] 内存与进程
来源：http://uxw.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://wvn.haohaochexian.top

[R64] 结束进程
来源：http://sek.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://rjf.redwolf501.top

[R65] 查看端口占用
来源：http://pyi.sweek.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://akt.yfazqb.com

[R66] 定时任务
来源：http://yrf.haohaochexian.top

crontab -e;  crontab -l
来源：http://hhs.xuanzx.com

[R67] 生成随机十六进制串
来源：http://vpq.cashguo.top

openssl rand -hex 16
来源：http://bys.jiagoushi.top

[R68] 计算文件校验值
来源：http://dsi.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://nrc.yongpay.top

[R69] 生成随机密码
来源：http://cne.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://iee.quarkkingdee.top

[R70] 时间戳与互转
来源：http://jmd.sxryk.cn

date +%s;  date -d @1700000000
来源：http://hjk.sjlbkw.cn

[R71] 日期格式化
来源：http://ymy.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jsz.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://gqf.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://brx.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://blc.ydjk.org.cn

split -l 1000 big.log part_
来源：http://ztf.uphjek.com

[R74] 批量重命名
来源：http://oyd.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ntg.feifeiyinyue.top

[R75] 导出环境变量
来源：http://gnz.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://vei.yongpay.top

[R76] 使用临时文件
来源：http://yta.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bcs.yuxming.cn

[R77] 读取用户输入
来源：http://gcr.gotoacloud.top

read -rp "请输入: " ans
来源：http://ibb.redwolf501.top

[R78] 交互式菜单
来源：http://jhu.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sqk.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://qiv.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pnt.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://brs.fanxiaobao.xyz

time ./run.sh
来源：http://xpn.jyoumei.cn

================================================================================
来源：http://pbn.fehbvm.com

S. C / C++ 专题
来源：http://axr.cheryme.top

================================================================================
来源：http://abs.tanke756.top

[S01] C：Hello World
来源：http://fba.jqgfzy.top

#include <stdio.h>
来源：http://lzf.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fmk.xuanzx.com

[S02] C：变量与格式化输出
来源：http://yfl.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://lur.fanxiaobao.xyz

[S03] C：读入整数
来源：http://vrt.zhixingplan.top

int x; scanf("%d", &x);
来源：http://uoa.hnxiangtu.top

[S04] C：字符串复制
来源：http://mqx.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sgd.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://vvt.daria6918.cn

strlen(s)
来源：http://jdj.gogol.net.cn

[S06] C：字符串比较
来源：http://wgj.sweek.top

strcmp(a, b) == 0
来源：http://lxx.fengsongda.top

[S07] C：数组遍历求和
来源：http://koy.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wsj.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://oqs.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vnv.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://tfj.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mrb.sxryk.cn

[S10] C：指针与解引用
来源：http://hcd.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://xts.shzxlz.cn

[S11] C：逐行读文件
来源：http://mka.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://vso.ctjpmb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://urq.zdqjudy.top

fclose(f);
来源：http://txz.hnxiangtu.top

[S12] C：写文件
来源：http://kyh.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pev.pengpengdd.cyou

[S13] C：宏定义
来源：http://atz.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lsf.yvedp.cn

[S14] C：枚举
来源：http://fdz.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://xxv.cqqwz.cn

[S15] C：类型转换
来源：http://juf.hammf.cn

(double) a / b
来源：http://orb.jianghu66.top

[S16] C：位操作置位
来源：http://nsn.jqgfzy.top

x |= (1 << 3);
来源：http://fqd.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://knv.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://njc.yueranfly.top

[S18] C：命令行参数
来源：http://sho.yangfankeji.com

int main(int argc, char **argv)
来源：http://gmj.gogol.net.cn

[S19] C：快速排序
来源：http://zbw.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://ieg.smart0.xyz

[S20] C：二分查找
来源：http://wqk.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rnr.fengsongda.top

[S21] C：字符类别判断
来源：http://tob.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dqr.cqqwz.cn

[S22] C：字符串转数字
来源：http://jqk.yj202588.top

atoi("42");  strtod("3.14", NULL);
来源：http://rkc.pycfn.com

[S23] C：随机数
来源：http://bbz.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://htl.sysykeji.top

[S24] C：获取本地时间
来源：http://ueu.hysaishi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jbs.yuxming.cn

[S25] C：内存拷贝
来源：http://oia.c1oappe.top

memcpy(dst, src, n);
来源：http://ghf.redwolf501.top

[S26] C：内存清零
来源：http://ech.mhx1999.top

memset(a, 0, sizeof a);
来源：http://kbd.gogol.net.cn

[S27] C：定义常量
来源：http://zbc.hammf.cn

const double PI = 3.14159;
来源：http://ail.ppjwa.cn

[S28] C：静态变量
来源：http://afz.yongpay.top

static int counter = 0;
来源：http://dpq.epnwcf.com

[S29] C：变参函数
来源：http://ebx.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lsu.jiagoushi.top

[S30] C：头文件保护
来源：http://dpp.dianchejie.cn

#ifndef X_H
来源：http://nqh.birdmap.top

#define X_H
来源：http://tdp.fehbvm.com

#endif
来源：http://fbj.ppjwa.cn

[S31] C++：Hello World
来源：http://jzm.shzxlz.cn

#include <iostream>
来源：http://ytk.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://zfr.shuidangran.top

[S32] C++：字符串
来源：http://pyw.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://xyk.uphjek.com

[S33] C++：vector 增删
来源：http://qjh.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dnx.yangfankeji.com

[S34] C++：遍历 vector
来源：http://rao.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://ofu.birdmap.top

[S35] C++：map
来源：http://won.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bvn.yj20258.top

[S36] C++：unordered_map
来源：http://shg.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wwn.havefunace.top

[S37] C++：set
来源：http://aky.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nyk.yangfankeji.com

[S38] C++：排序
来源：http://qhp.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://wrc.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://yuq.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mas.epnwcf.com

[S40] C++：查找元素
来源：http://kxl.yj20258.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zpw.shuidangran.top

[S41] C++：类与构造函数
来源：http://aep.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bja.hcnkem.com

[S42] C++：继承与虚函数
来源：http://duq.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://zna.tianlin.xyz

[S43] C++：智能指针
来源：http://xpx.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://rqs.316326.xyz

[S44] C++：引用传参
来源：http://dmi.wangdashe.top

void inc(int &x) { ++x; }
来源：http://hzf.sjlbkw.cn

[S45] C++：lambda
来源：http://irs.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://umk.fktsv.cn

[S46] C++：函数模板
来源：http://vyq.aibaodan.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hgt.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://hwq.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dfq.wangdashe.top

[S48] C++：逐行读文件
来源：http://abt.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://mpo.mhx1999.top

while (std::getline(in, line)) { }
来源：http://wgv.chenzaomai.com

[S49] C++：写文件
来源：http://ymh.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ibp.epnwcf.com

[S50] C++：格式化数字
来源：http://mdi.iojbl.cn


<!-- 参考信息 -->