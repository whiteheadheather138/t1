代发 wailian999

[Q78] 当前时间
来源：http://nzz.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://adi.svipenyu.cn

[Q79] 字符串拼接
来源：http://evo.guowangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uch.nwbrower.top

[Q80] 字符串截取
来源：http://fes.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iun.jlsjyb.cn

[Q81] 字符串替换
来源：http://xuf.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nmg.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://esy.hysaishi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hyz.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://nag.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gvv.andypj.xyz

[Q84] 去除首尾空格
来源：http://dki.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://sjs.aizwys.cn

[Q85] 数值取整
来源：http://gxu.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cop.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://zok.jinqigfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tcg.cheryme.top

[Q87] JSON 字段做条件
来源：http://kkh.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cqy.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://rbt.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eta.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eyc.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://gfd.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hnh.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://hgn.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ajb.yuxming.cn

================================================================================
来源：http://ghp.zhongyouzk.top

R. Bash 专题
来源：http://yls.jqgufenzy.top

================================================================================
来源：http://vqe.yj20258.top

[R01] shebang 与严格模式
来源：http://uow.ehwqpu.com

#!/usr/bin/env bash
来源：http://hvu.aibaodan.cn

set -euo pipefail
来源：http://llq.316326.xyz

[R02] 变量赋值与使用
来源：http://biy.birdmap.top

name="Tom"; echo "$name"
来源：http://adz.yongpay.top

[R03] 只读变量
来源：http://hdi.zhixingplan.top

readonly PI=3.14
来源：http://idc.shuidangran.top

[R04] 位置参数
来源：http://rjj.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ajm.yongpay.top

[R05] 参数默认值
来源：http://nry.shanyushiyangtech.top

name="${1:-default}"
来源：http://czf.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://smo.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tap.pengpengdd.cyou

[R07] if 判断文件
来源：http://eil.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xks.52xcode.cn

[R08] 数值比较
来源：http://arv.gaohongyu789.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zhq.redwolf501.top

[R09] 字符串比较
来源：http://ezo.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ptm.gaohongyu789.top

[R10] 正则匹配
来源：http://ihw.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wrx.aibaodan.cn

[R11] case 多分支
来源：http://ekt.hammf.cn

case "$1" in
来源：http://sfs.chenjidiqi.icu

start) echo "启动" ;;
来源：http://pdj.yj20258.top

stop)  echo "停止" ;;
来源：http://eim.sxryk.cn

*)     echo "未知命令" ;;
来源：http://txb.hongshengwenyu.top

esac
来源：http://mwl.vqdsnc.cn

[R12] for 遍历文件
来源：http://wqn.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://yxi.ehwqpu.com

[R13] for 计数循环
来源：http://hoy.smart0.xyz

for i in {1..10}; do echo "$i"; done
来源：http://qad.yuanzhike.top

[R14] C 风格 for
来源：http://hia.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nfx.birdmap.top

[R15] while 逐行读文件
来源：http://imt.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tor.birdmap.top

[R16] until 等待条件
来源：http://vwb.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nmj.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://vbw.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://fsm.nwbrower.top

[R18] 遍历数组
来源：http://aym.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qza.sufxvd.cn

[R19] 数组长度
来源：http://kcr.chenlongwang.top

echo "${#arr[@]}"
来源：http://mvh.shanyushiyangtech.top

[R20] 关联数组（字典）
来源：http://vsn.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kxo.tian-w.cn

[R21] 字符串长度
来源：http://scu.bjfxy.top

echo "${#s}"
来源：http://mli.nwbrower.top

[R22] 截取子串
来源：http://nql.ydjk.org.cn

echo "${s:0:5}"
来源：http://zah.jinqigfzy.top

[R23] 字符串替换
来源：http://pqg.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uim.daria6918.cn

[R24] 大小写转换
来源：http://app.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://uqk.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://dfj.dashuyun.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gco.zdbjq.cn

[R26] 命令替换
来源：http://fmk.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://mwe.yangfankeji.com

[R27] 算术展开
来源：http://vaz.ivvv.top

echo $((1 + 2 * 3))
来源：http://ghy.gzhubu.top

[R28] 浮点运算
来源：http://tdm.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://onp.cheryme.top

[R29] 定义函数
来源：http://zpt.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yyp.havefunace.top

[R30] 函数返回状态码
来源：http://iyl.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://jau.daxiang520.top

[R31] 局部变量
来源：http://jjj.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://ztr.yongpay.top

[R32] 参数个数校验
来源：http://kzj.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bqy.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://qqw.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cgb.ctjpmb.com

[R34] 退出时清理
来源：http://app.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://tmw.hfpthk.cn

[R35] 后台执行并等待
来源：http://sbt.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://djc.hfpthk.cn

[R36] 并发执行多个任务
来源：http://lul.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lfn.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://wbj.0kj1m.cn

files=$(ls -1)
来源：http://yjc.birdmap.top

[R38] 管道串联
来源：http://usd.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://tzi.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://ike.havefunace.top

cmd > out.log 2>&1
来源：http://qpy.ydjk.org.cn

[R40] 追加写日志
来源：http://pod.fktsv.cn

echo "log" >> out.log
来源：http://orc.jqgufenzy.top

[R41] 丢弃输出
来源：http://viw.52xcode.cn

cmd >/dev/null 2>&1
来源：http://xmg.wangdashe.top

[R42] 输入重定向
来源：http://hby.yj202588.top

wc -l < a.txt
来源：http://dqp.vehdjk.com

[R43] 按名字查找文件
来源：http://ivd.nanxinkj.top

find . -name "*.log" -type f
来源：http://xkw.fktsv.cn

[R44] 按修改时间查找
来源：http://bei.havefunace.top

find . -mtime -7 -type f
来源：http://qsm.chenlongwang.top

[R45] 批量删除
来源：http://dcn.aizwys.cn

find . -name "*.tmp" -delete
来源：http://btf.guannengcc.top

[R46] 递归替换文件内容
来源：http://wzh.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fmn.sysykeji.top

[R47] sed 单行替换
来源：http://fmi.haohaochexian.top

sed -i 's/foo/bar/g' a.txt
来源：http://jwa.andypj.xyz

[R48] awk 取指定列
来源：http://gzp.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://dfa.aibaodan.cn

[R49] awk 带条件
来源：http://iwi.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vdx.kuanghao11.cn

[R50] awk 求和
来源：http://npr.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://zlr.havefunace.top

[R51] 排序去重取前几
来源：http://jxk.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://kty.kuanghao11.cn

[R52] 统计行数
来源：http://rrz.guannengcc.top

wc -l a.txt
来源：http://rwa.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://wwe.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jrc.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://sfv.ydjk.org.cn

diff a.txt b.txt
来源：http://wrp.ctjpmb.com

[R55] 压缩与解压
来源：http://yvx.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ypn.vqdsnc.cn

[R56] 远程拷贝
来源：http://wwn.hywenlv.cn

scp file user@host:/path/
来源：http://cif.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://mjd.hnqzz.top

ssh user@host 'uptime'
来源：http://dcs.tanke756.top

[R58] 下载文件
来源：http://jhx.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ttj.ydzc1.top

[R59] 发 POST JSON
来源：http://fwq.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://big.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://phj.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://umn.ehwqpu.com

[R61] 磁盘占用
来源：http://bmn.shuidangran.top

df -h;  du -sh *
来源：http://izt.yueranfly.top

[R62] 找最占空间的文件
来源：http://lkr.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://ugn.0kj1m.cn

[R63] 内存与进程
来源：http://fxf.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://ewz.sweek.top

[R64] 结束进程
来源：http://eln.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://sur.bjfxy.top

[R65] 查看端口占用
来源：http://msj.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uyy.ivvv.top

[R66] 定时任务
来源：http://dly.gotoacloud.top

crontab -e;  crontab -l
来源：http://qae.jyoumei.cn

[R67] 生成随机十六进制串
来源：http://eyd.xuanzx.com

openssl rand -hex 16
来源：http://lzc.cdnleiting.top

[R68] 计算文件校验值
来源：http://jix.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://cyz.zhengqikj.top

[R69] 生成随机密码
来源：http://ekm.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://gup.wangdashe.top

[R70] 时间戳与互转
来源：http://aqt.xinyue.icu

date +%s;  date -d @1700000000
来源：http://tht.ybcxt.top

[R71] 日期格式化
来源：http://gdg.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://boy.yangfankeji.com

[R72] 等待端口就绪
来源：http://bdx.mhx1999.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qul.sweek.top

[R73] 分割大日志
来源：http://xwo.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://jqm.wangdashe.top

[R74] 批量重命名
来源：http://pcz.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jpb.zhijiandao.cn

[R75] 导出环境变量
来源：http://gjb.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://dav.wangshuangyany.cn

[R76] 使用临时文件
来源：http://xzy.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eeh.bjfxy.top

[R77] 读取用户输入
来源：http://yli.xziqi.cn

read -rp "请输入: " ans
来源：http://eby.hammf.cn

[R78] 交互式菜单
来源：http://qxn.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nao.gotoacloud.top

[R79] 解析命令行选项
来源：http://flq.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://whh.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://ali.cheryme.top

time ./run.sh
来源：http://mlq.jlsjyb.cn

================================================================================
来源：http://tgs.ydjk.org.cn

S. C / C++ 专题
来源：http://tew.yongpay.top

================================================================================
来源：http://vxm.gzhubu.top

[S01] C：Hello World
来源：http://iue.meibo888.top

#include <stdio.h>
来源：http://dqd.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://icj.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://ded.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://iax.havefunace.top

[S03] C：读入整数
来源：http://wpp.sysykeji.top

int x; scanf("%d", &x);
来源：http://nek.chenjidiqi.icu

[S04] C：字符串复制
来源：http://xwo.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://txq.0kj1m.cn

[S05] C：字符串长度
来源：http://ohw.ppjwa.cn

strlen(s)
来源：http://xrg.ydzc1.top

[S06] C：字符串比较
来源：http://kqk.gogol.net.cn

strcmp(a, b) == 0
来源：http://mtz.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://psv.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ben.cdnleiting.top

[S08] C：动态内存分配与释放
来源：http://irn.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uog.havefunace.top

[S09] C：结构体定义与初始化
来源：http://mna.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://efv.sufxvd.cn

[S10] C：指针与解引用
来源：http://kyb.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://ono.nanxuanxn.top

[S11] C：逐行读文件
来源：http://lwn.yongpay.top

FILE *f = fopen("a.txt", "r");
来源：http://pmn.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://uia.cdnleiting.top

fclose(f);
来源：http://wlz.hesvh.cn

[S12] C：写文件
来源：http://kso.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pze.jlsjyb.cn

[S13] C：宏定义
来源：http://tao.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dhq.xylfe.cn

[S14] C：枚举
来源：http://yvz.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://svx.yuanzhike.top

[S15] C：类型转换
来源：http://xez.iojbl.cn

(double) a / b
来源：http://eku.guannengcc.top

[S16] C：位操作置位
来源：http://txq.smart0.xyz

x |= (1 << 3);
来源：http://xyq.redwolf501.top

[S17] C：安全拼接字符串
来源：http://inp.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zkz.ydzc1.top

[S18] C：命令行参数
来源：http://zrc.yonumen.top

int main(int argc, char **argv)
来源：http://qaq.vehdjk.com

[S19] C：快速排序
来源：http://fsv.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pun.chenlongwang.top

[S20] C：二分查找
来源：http://ixn.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iyj.gotoacloud.top

[S21] C：字符类别判断
来源：http://kwo.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iyg.pycfn.com

[S22] C：字符串转数字
来源：http://amg.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://pxr.cdnleiting.top

[S23] C：随机数
来源：http://jby.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wqb.pycfn.com

[S24] C：获取本地时间
来源：http://qls.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bae.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://hop.jqgufenzy.top

memcpy(dst, src, n);
来源：http://qmf.vqdsnc.cn

[S26] C：内存清零
来源：http://rxz.xylfe.cn

memset(a, 0, sizeof a);
来源：http://rnj.ybcxt.top

[S27] C：定义常量
来源：http://thg.jianghu66.top

const double PI = 3.14159;
来源：http://fcp.cdnleiting.top

[S28] C：静态变量
来源：http://hpr.wangshuangyany.cn

static int counter = 0;
来源：http://gms.jlsjyb.cn

[S29] C：变参函数
来源：http://uis.nanxinkj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iev.xuetiantiany.cn

[S30] C：头文件保护
来源：http://tns.52xcode.cn

#ifndef X_H
来源：http://gxk.sufxvd.cn

#define X_H
来源：http://yfx.fktsv.cn

#endif
来源：http://rad.yuxming.cn

[S31] C++：Hello World
来源：http://xde.chenzaomai.com

#include <iostream>
来源：http://mlt.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://jfx.zhengqikj.top

[S32] C++：字符串
来源：http://ysi.yongpay.top

std::string s = "hi";  s += "!";
来源：http://irw.nwbrower.top

[S33] C++：vector 增删
来源：http://gdo.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bbi.hcnkem.com

[S34] C++：遍历 vector
来源：http://iwx.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://bec.shzxlz.cn

[S35] C++：map
来源：http://myn.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://onk.ivvv.top

[S36] C++：unordered_map
来源：http://vev.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rhi.meibo888.top

[S37] C++：set
来源：http://xiq.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wlm.zdqjudy.top

[S38] C++：排序
来源：http://zlx.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://pls.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://ozt.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ksi.jlsjyb.cn

[S40] C++：查找元素
来源：http://uvy.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bss.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://dcg.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uyb.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://xji.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://lib.ctjpmb.com

[S43] C++：智能指针
来源：http://csf.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://hcr.jqgufenzy.top

[S44] C++：引用传参
来源：http://aog.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://mab.yonumen.top

[S45] C++：lambda
来源：http://ezd.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://duj.nanxuanxn.top

[S46] C++：函数模板
来源：http://tbo.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qxo.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://eeh.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bne.yonumen.top

[S48] C++：逐行读文件
来源：http://ofa.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://pdo.andypj.xyz


<!-- 参考信息 -->