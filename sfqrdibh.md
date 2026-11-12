代发 wailian999

[Q78] 当前时间
来源：http://zet.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fzp.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://snv.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lsq.fengsongda.top

[Q80] 字符串截取
来源：http://rit.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ryr.haohaochexian.top

[Q81] 字符串替换
来源：http://yzx.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ldd.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://cqm.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qxz.cashguo.top

[Q83] 大小写转换
来源：http://cbs.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lgp.chenzaomai.com

[Q84] 去除首尾空格
来源：http://shp.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://fsp.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://arc.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xpa.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://hfv.ctjpmb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gwu.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://zxa.zhengqikj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vfs.jiagoushi.top

[Q88] 行转列（条件聚合）
来源：http://nkw.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yop.zhijiandao.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ljz.xziqi.cn

[Q89] 判断表是否存在
来源：http://upy.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://epe.ybcxt.top

[Q90] 生成序号列
来源：http://afo.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gvh.fzhhl.top

================================================================================
来源：http://hhh.kuanghao11.cn

R. Bash 专题
来源：http://szf.yueranfly.top

================================================================================
来源：http://zre.zhixingplan.top

[R01] shebang 与严格模式
来源：http://ldp.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://vye.chenjidiqi.icu

set -euo pipefail
来源：http://kwo.hnqzz.top

[R02] 变量赋值与使用
来源：http://olc.cdnleiting.top

name="Tom"; echo "$name"
来源：http://kjq.guannengcc.top

[R03] 只读变量
来源：http://lcb.chenzaomai.com

readonly PI=3.14
来源：http://tsp.shanyushiyangtech.top

[R04] 位置参数
来源：http://yio.chenjidiqi.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nur.jinqigfzy.top

[R05] 参数默认值
来源：http://ksb.yj20258.top

name="${1:-default}"
来源：http://unj.sweek.top

[R06] 判断命令是否存在
来源：http://lmb.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ptx.shangyingyoupin.top

[R07] if 判断文件
来源：http://cjo.52xcode.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vcj.hnxiangtu.top

[R08] 数值比较
来源：http://gby.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nky.aizwys.cn

[R09] 字符串比较
来源：http://ooq.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://udo.ehwqpu.com

[R10] 正则匹配
来源：http://mqy.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ong.gaohongyu789.top

[R11] case 多分支
来源：http://bnm.sysykeji.top

case "$1" in
来源：http://gxs.hongshengwenyu.top

start) echo "启动" ;;
来源：http://xsa.cucudq.cn

stop)  echo "停止" ;;
来源：http://kgb.jqgfzy.top

*)     echo "未知命令" ;;
来源：http://qvt.nanxinkj.top

esac
来源：http://wok.aibaodan.cn

[R12] for 遍历文件
来源：http://ubd.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://vry.shanyushiyangkeji.top

[R13] for 计数循环
来源：http://oko.xuetiantiany.cn

for i in {1..10}; do echo "$i"; done
来源：http://nhn.cqqwz.cn

[R14] C 风格 for
来源：http://lbm.nanxuanxn.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://djw.chenzaomai.com

[R15] while 逐行读文件
来源：http://wvf.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://its.yuanzhike.top

[R16] until 等待条件
来源：http://iea.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gvs.chenlongwang.top

[R17] 数组定义与取值
来源：http://ofq.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://ojx.ydjk.org.cn

[R18] 遍历数组
来源：http://zqm.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vmt.ehwqpu.com

[R19] 数组长度
来源：http://qik.hnxiangtu.top

echo "${#arr[@]}"
来源：http://gqu.havefunace.top

[R20] 关联数组（字典）
来源：http://ebu.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://djr.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://anq.gaohongyu789.top

echo "${#s}"
来源：http://ape.jiagoushi.top

[R22] 截取子串
来源：http://umk.epnwcf.com

echo "${s:0:5}"
来源：http://olh.ppjwa.cn

[R23] 字符串替换
来源：http://tml.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tdw.hesvh.cn

[R24] 大小写转换
来源：http://alg.hcnkem.com

echo "${s^^}"; echo "${s,,}"
来源：http://iwy.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://seb.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://nvv.jinqigufen.top

[R26] 命令替换
来源：http://idr.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://pwc.cashguo.top

[R27] 算术展开
来源：http://prc.tarul.cn

echo $((1 + 2 * 3))
来源：http://lam.zhijiandao.cn

[R28] 浮点运算
来源：http://orv.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://tzx.cashguo.top

[R29] 定义函数
来源：http://ptv.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nsn.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://grf.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://sry.chenjidiqi.icu

[R31] 局部变量
来源：http://kyr.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://hgb.jinghuilouyu.cn

[R32] 参数个数校验
来源：http://xop.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kod.cashguo.top

[R33] 捕获错误并提示行号
来源：http://nwz.jianghu66.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://txh.cheryme.top

[R34] 退出时清理
来源：http://nxg.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://xfl.yuanzhike.top

[R35] 后台执行并等待
来源：http://dlr.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://oen.zhengqikj.top

[R36] 并发执行多个任务
来源：http://odv.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://frm.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://ryc.jianghu66.top

files=$(ls -1)
来源：http://oze.yj20258.top

[R38] 管道串联
来源：http://cjb.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://fia.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://trv.yj20258.top

cmd > out.log 2>&1
来源：http://aid.jianghu66.top

[R40] 追加写日志
来源：http://sez.aizwys.cn

echo "log" >> out.log
来源：http://uzg.jqgufenzy.top

[R41] 丢弃输出
来源：http://wuz.tian-w.cn

cmd >/dev/null 2>&1
来源：http://ehu.hongshengwenyu.top

[R42] 输入重定向
来源：http://crh.uphjek.com

wc -l < a.txt
来源：http://mnw.sysykeji.top

[R43] 按名字查找文件
来源：http://tlu.yonumen.top

find . -name "*.log" -type f
来源：http://egp.xziqi.cn

[R44] 按修改时间查找
来源：http://pid.hfpthk.cn

find . -mtime -7 -type f
来源：http://gsc.iojbl.cn

[R45] 批量删除
来源：http://eas.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://tqr.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://aih.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lso.mhx1999.top

[R47] sed 单行替换
来源：http://ubu.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mqo.ehwqpu.com

[R48] awk 取指定列
来源：http://pws.sweek.top

awk '{print $1, $3}' a.txt
来源：http://ccp.bjfxy.top

[R49] awk 带条件
来源：http://gel.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://paw.haohaochexian.top

[R50] awk 求和
来源：http://dzg.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://jby.jyoumei.cn

[R51] 排序去重取前几
来源：http://mis.quarkkingdee.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vpv.xinyue.icu

[R52] 统计行数
来源：http://wfy.xuetiantiany.cn

wc -l a.txt
来源：http://dzh.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://sdz.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fax.cdnleiting.top

[R54] 比较两个文件
来源：http://xcv.shanyushiyangtech.top

diff a.txt b.txt
来源：http://axm.ybcxt.top

[R55] 压缩与解压
来源：http://eow.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ako.hesvh.cn

[R56] 远程拷贝
来源：http://liy.yueranfly.top

scp file user@host:/path/
来源：http://dmt.feifeiyinyue.top

[R57] 远程执行命令
来源：http://elo.gaohongyu789.top

ssh user@host 'uptime'
来源：http://ncs.chenzaomai.com

[R58] 下载文件
来源：http://lkp.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sdf.hywenlv.cn

[R59] 发 POST JSON
来源：http://sla.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hxl.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://lvk.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zrc.hongshengwenyu.top

[R61] 磁盘占用
来源：http://ckc.hywenlv.cn

df -h;  du -sh *
来源：http://iwn.zdqjudy.top

[R62] 找最占空间的文件
来源：http://guf.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://ksp.gogol.net.cn

[R63] 内存与进程
来源：http://nna.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://xdv.ydjk.org.cn

[R64] 结束进程
来源：http://ocx.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://owo.yonumen.top

[R65] 查看端口占用
来源：http://luv.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oah.hfpthk.cn

[R66] 定时任务
来源：http://sre.tarul.cn

crontab -e;  crontab -l
来源：http://ygy.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://ecq.dashuyun.cn

openssl rand -hex 16
来源：http://gvs.zhijiandao.cn

[R68] 计算文件校验值
来源：http://vqn.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://jrx.jiagoushi.top

[R69] 生成随机密码
来源：http://wou.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://zna.sysykeji.top

[R70] 时间戳与互转
来源：http://zqk.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://wva.cheryme.top

[R71] 日期格式化
来源：http://yug.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://xfg.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://izh.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xxk.yvedp.cn

[R73] 分割大日志
来源：http://xvc.zhongyouzk.top

split -l 1000 big.log part_
来源：http://ceb.ydjk.org.cn

[R74] 批量重命名
来源：http://wfb.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ntf.cashguo.top

[R75] 导出环境变量
来源：http://klr.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://koe.pengpengdd.cyou

[R76] 使用临时文件
来源：http://vcy.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pxw.fktsv.cn

[R77] 读取用户输入
来源：http://wfo.ctjpmb.com

read -rp "请输入: " ans
来源：http://nws.vqdsnc.cn

[R78] 交互式菜单
来源：http://sui.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ccf.jinqigufen.top

[R79] 解析命令行选项
来源：http://agt.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lhi.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://opp.snrcjt.cn

time ./run.sh
来源：http://ahg.jinqigfzy.top

================================================================================
来源：http://itx.bjfxy.top

S. C / C++ 专题
来源：http://jzo.gaohongyu789.top

================================================================================
来源：http://frt.jyoumei.cn

[S01] C：Hello World
来源：http://igw.shanyushiyangkeji.top

#include <stdio.h>
来源：http://xjs.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rwj.yj202588.top

[S02] C：变量与格式化输出
来源：http://kgi.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://opq.zhijiandao.cn

[S03] C：读入整数
来源：http://yrd.hcnkem.com

int x; scanf("%d", &x);
来源：http://hiu.nwbrower.top

[S04] C：字符串复制
来源：http://ymv.ydjk.org.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zvt.guowangkeji.top

[S05] C：字符串长度
来源：http://hfc.wangdashe.top

strlen(s)
来源：http://tdb.redwolf501.top

[S06] C：字符串比较
来源：http://xwv.yvedp.cn

strcmp(a, b) == 0
来源：http://ksr.zdqjudy.top

[S07] C：数组遍历求和
来源：http://nef.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wub.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://svz.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fyd.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://iny.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xzx.fzhhl.top

[S10] C：指针与解引用
来源：http://qle.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://nus.jiagoushi.top

[S11] C：逐行读文件
来源：http://cve.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://wcq.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://qbp.gogol.net.cn

fclose(f);
来源：http://mgf.tanke756.top

[S12] C：写文件
来源：http://pwh.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://krf.zhaomingkeji.xyz

[S13] C：宏定义
来源：http://kus.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dbf.52xcode.cn

[S14] C：枚举
来源：http://hka.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://rsf.havefunace.top

[S15] C：类型转换
来源：http://kxd.guannengcc.top

(double) a / b
来源：http://ckb.havefunace.top

[S16] C：位操作置位
来源：http://kwq.jiagoushi.top

x |= (1 << 3);
来源：http://guv.wangdashe.top

[S17] C：安全拼接字符串
来源：http://uop.fktsv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sos.sxryk.cn

[S18] C：命令行参数
来源：http://aau.fzhhl.top

int main(int argc, char **argv)
来源：http://vkl.meibo888.top

[S19] C：快速排序
来源：http://ujn.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ate.yj202588.top

[S20] C：二分查找
来源：http://jkj.xylfe.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zbi.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://wna.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ojl.xylfe.cn

[S22] C：字符串转数字
来源：http://jyg.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://byi.gotoacloud.top

[S23] C：随机数
来源：http://bvl.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sul.fengsongda.top

[S24] C：获取本地时间
来源：http://dlc.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://exe.shzxlz.cn

[S25] C：内存拷贝
来源：http://uqz.ybcxt.top

memcpy(dst, src, n);
来源：http://tcg.hongshengwenyu.top

[S26] C：内存清零
来源：http://kxh.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://ljw.zdbjq.cn

[S27] C：定义常量
来源：http://nnx.dashuyun.cn

const double PI = 3.14159;
来源：http://qxs.52xcode.cn

[S28] C：静态变量
来源：http://cww.9152youxi.cn

static int counter = 0;
来源：http://ycx.yonumen.top

[S29] C：变参函数
来源：http://dur.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mkz.xinyue.icu

[S30] C：头文件保护
来源：http://ema.cheryme.top

#ifndef X_H
来源：http://lho.nwbrower.top

#define X_H
来源：http://khq.zhaomingkeji.xyz

#endif
来源：http://zym.shuidangran.top

[S31] C++：Hello World
来源：http://zkj.tian-w.cn

#include <iostream>
来源：http://xqg.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://hse.birdmap.top

[S32] C++：字符串
来源：http://ntn.yj20258888.top

std::string s = "hi";  s += "!";
来源：http://tlm.tanke756.top

[S33] C++：vector 增删
来源：http://qhr.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qef.yvedp.cn

[S34] C++：遍历 vector
来源：http://ukt.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://zru.fktsv.cn

[S35] C++：map
来源：http://miw.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lnq.fzhhl.top

[S36] C++：unordered_map
来源：http://afq.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hnl.hesvh.cn

[S37] C++：set
来源：http://gno.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mfp.hfpthk.cn

[S38] C++：排序
来源：http://wjw.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://mli.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://jre.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gim.yuxming.cn

[S40] C++：查找元素
来源：http://oyc.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xxv.meibo888.top

[S41] C++：类与构造函数
来源：http://sas.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gti.hammf.cn

[S42] C++：继承与虚函数
来源：http://ggv.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://bgv.ivvv.top

[S43] C++：智能指针
来源：http://qoy.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://goj.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://xtx.mhx1999.top

void inc(int &x) { ++x; }
来源：http://kce.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://nri.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://bij.smart0.xyz

[S46] C++：函数模板
来源：http://xde.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://obs.hesvh.cn

[S47] C++：结构化绑定遍历
来源：http://dku.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wer.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://aos.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://fud.gaohongyu789.top


<!-- 参考信息 -->