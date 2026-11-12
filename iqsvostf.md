代发 wailian999

ROLLBACK TO sp1;
来源：http://dzg.zdbjq.cn

[Q69] 查看执行计划
来源：http://vki.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xvn.ybcxt.top

[Q70] 更新统计信息
来源：http://tjy.chenjidiqi.icu

ANALYZE TABLE users;
来源：http://yrc.ppjwa.cn

[Q71] 查看建表语句
来源：http://qru.cashguo.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vex.gogol.net.cn

[Q72] 查看索引
来源：http://bdq.yongpay.top

SHOW INDEX FROM users;
来源：http://lyi.gogol.net.cn

[Q73] 查看表状态
来源：http://xgr.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fjf.mhx1999.top

[Q74] 强制使用索引
来源：http://ipw.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fnu.yonumen.top

[Q75] 日期格式化
来源：http://snm.zycfv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pez.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fgk.sysykeji.top

[Q76] 按天统计
来源：http://hii.vehdjk.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vwm.nwbrower.top

[Q77] 时间加减
来源：http://gal.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dhg.xuetiantiany.cn

[Q78] 当前时间
来源：http://yvl.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lin.9152youxi.cn

[Q79] 字符串拼接
来源：http://cim.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uuf.xylfe.cn

[Q80] 字符串截取
来源：http://wwo.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yvx.meibo888.top

[Q81] 字符串替换
来源：http://yvl.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mni.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://wty.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tjh.haohaochexian.top

[Q83] 大小写转换
来源：http://bcq.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cen.daxiang520.top

[Q84] 去除首尾空格
来源：http://jim.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://dfu.316326.xyz

[Q85] 数值取整
来源：http://nic.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hbg.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://aoc.nanxuanxn.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ppw.tarul.cn

[Q87] JSON 字段做条件
来源：http://jsh.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hdd.jinyuanbaomall.cn

[Q88] 行转列（条件聚合）
来源：http://fcx.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://feu.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zwd.9152youxi.cn

[Q89] 判断表是否存在
来源：http://nxm.tarul.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://giv.9152youxi.cn

[Q90] 生成序号列
来源：http://jix.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://usy.ywan-chungtsiang.top

================================================================================
来源：http://thz.ivvv.top

R. Bash 专题
来源：http://lda.chenlongwang.top

================================================================================
来源：http://xcm.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://ehn.ydjk.org.cn

#!/usr/bin/env bash
来源：http://lcr.nanxuanxn.top

set -euo pipefail
来源：http://qdf.vehdjk.com

[R02] 变量赋值与使用
来源：http://ery.yuanzhike.top

name="Tom"; echo "$name"
来源：http://knm.zycfv.cn

[R03] 只读变量
来源：http://dhy.feifeiyinyue.top

readonly PI=3.14
来源：http://dtf.52xcode.cn

[R04] 位置参数
来源：http://nkh.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eol.wangshuangyany.cn

[R05] 参数默认值
来源：http://qai.yueranfly.top

name="${1:-default}"
来源：http://cjl.0kj1m.cn

[R06] 判断命令是否存在
来源：http://pmz.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lfm.gotoacloud.top

[R07] if 判断文件
来源：http://lmw.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://edq.fktsv.cn

[R08] 数值比较
来源：http://yla.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://vdq.jyoumei.cn

[R09] 字符串比较
来源：http://egt.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vhm.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://tns.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://orh.epnwcf.com

[R11] case 多分支
来源：http://xnj.meibo888.top

case "$1" in
来源：http://bff.zhijiandao.cn

start) echo "启动" ;;
来源：http://jyn.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://ndz.52xcode.cn

*)     echo "未知命令" ;;
来源：http://snc.chenjidiqi.icu

esac
来源：http://xqw.bbcook.cn

[R12] for 遍历文件
来源：http://mus.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://rmq.aizwys.cn

[R13] for 计数循环
来源：http://vnq.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://zrb.mhx1999.top

[R14] C 风格 for
来源：http://kze.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eai.hammf.cn

[R15] while 逐行读文件
来源：http://vwg.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sfh.yj202588.top

[R16] until 等待条件
来源：http://xpx.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ahb.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://teb.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://mvw.wangshuangyany.cn

[R18] 遍历数组
来源：http://ccu.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://akg.tian-w.cn

[R19] 数组长度
来源：http://nly.jqgufenzy.top

echo "${#arr[@]}"
来源：http://crk.ppjwa.cn

[R20] 关联数组（字典）
来源：http://eou.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nkb.pycfn.com

[R21] 字符串长度
来源：http://ush.shzxlz.cn

echo "${#s}"
来源：http://vxn.sweek.top

[R22] 截取子串
来源：http://gco.meibo888.top

echo "${s:0:5}"
来源：http://mgh.yanxiufei.cn

[R23] 字符串替换
来源：http://zcj.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kkj.hnxiangtu.top

[R24] 大小写转换
来源：http://aho.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bea.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://fqb.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://hjk.hfpthk.cn

[R26] 命令替换
来源：http://yvv.tianlin.xyz

now=$(date +%F); echo "$now"
来源：http://aks.snrcjt.cn

[R27] 算术展开
来源：http://ksr.yonumen.top

echo $((1 + 2 * 3))
来源：http://sff.tian-w.cn

[R28] 浮点运算
来源：http://bst.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://sfi.9152youxi.cn

[R29] 定义函数
来源：http://wuf.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yaq.pycfn.com

[R30] 函数返回状态码
来源：http://agw.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://jss.xinyue.icu

[R31] 局部变量
来源：http://xkn.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://hbu.xuetiantiany.cn

[R32] 参数个数校验
来源：http://vdf.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tzz.tarul.cn

[R33] 捕获错误并提示行号
来源：http://bdz.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hzy.yonumen.top

[R34] 退出时清理
来源：http://fzt.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://fpm.nwbrower.top

[R35] 后台执行并等待
来源：http://hqv.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pdh.guannengcc.top

[R36] 并发执行多个任务
来源：http://vsv.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gmq.haohaochexian.top

[R37] 把输出赋给变量
来源：http://ngf.yfazqb.com

files=$(ls -1)
来源：http://dxu.nanxuanxn.top

[R38] 管道串联
来源：http://owa.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://ahq.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://twl.sjlbkw.cn

cmd > out.log 2>&1
来源：http://rfr.xuanzx.com

[R40] 追加写日志
来源：http://pqr.gzhubu.top

echo "log" >> out.log
来源：http://gep.cdnleiting.top

[R41] 丢弃输出
来源：http://ehy.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://rgb.zhiwuduotai.top

[R42] 输入重定向
来源：http://dni.jianghu66.top

wc -l < a.txt
来源：http://wgs.mhx1999.top

[R43] 按名字查找文件
来源：http://eug.yj20258888.top

find . -name "*.log" -type f
来源：http://llc.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://jyh.jinqigufen.top

find . -mtime -7 -type f
来源：http://vfa.zhixingplan.top

[R45] 批量删除
来源：http://bbt.52xcode.cn

find . -name "*.tmp" -delete
来源：http://onn.hysaishi.cn

[R46] 递归替换文件内容
来源：http://wol.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hlf.gzhubu.top

[R47] sed 单行替换
来源：http://stt.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jmf.shangyingyoupin.top

[R48] awk 取指定列
来源：http://sbg.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://tqy.fktsv.cn

[R49] awk 带条件
来源：http://agq.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bqc.ivvv.top

[R50] awk 求和
来源：http://hyj.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://eex.jqgfzy.top

[R51] 排序去重取前几
来源：http://uif.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://atc.jqgufenzy.top

[R52] 统计行数
来源：http://cku.fengsongda.top

wc -l a.txt
来源：http://adj.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://ohr.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fbx.jinqigfzy.top

[R54] 比较两个文件
来源：http://qmd.zhongyouzk.top

diff a.txt b.txt
来源：http://bbc.zhijiandao.cn

[R55] 压缩与解压
来源：http://ejx.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yot.zhijiandao.cn

[R56] 远程拷贝
来源：http://wse.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://amw.hongshengwenyu.top

[R57] 远程执行命令
来源：http://xds.gotoacloud.top

ssh user@host 'uptime'
来源：http://erp.jlsjyb.cn

[R58] 下载文件
来源：http://txh.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eug.redwolf501.top

[R59] 发 POST JSON
来源：http://ihw.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lsq.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://lwa.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://snn.haohaochexian.top

[R61] 磁盘占用
来源：http://fcd.chenlongwang.top

df -h;  du -sh *
来源：http://vks.jinqigufen.top

[R62] 找最占空间的文件
来源：http://uih.meibo888.top

du -ah . | sort -rh | head -10
来源：http://dki.zycfv.cn

[R63] 内存与进程
来源：http://vrr.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://gdp.cqqwz.cn

[R64] 结束进程
来源：http://wgd.dianchejie.cn

kill -9 $(pgrep -f app.py)
来源：http://upj.aizwys.cn

[R65] 查看端口占用
来源：http://suy.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hal.shangyingyoupin.top

[R66] 定时任务
来源：http://wke.jlsjyb.cn

crontab -e;  crontab -l
来源：http://mxf.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://leq.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://vnz.meibo888.top

[R68] 计算文件校验值
来源：http://svn.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://oqb.gaohongyu789.top

[R69] 生成随机密码
来源：http://hmu.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://ofe.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://ofq.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://ehm.sxryk.cn

[R71] 日期格式化
来源：http://xru.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hof.zdqjudy.top

[R72] 等待端口就绪
来源：http://mvw.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fhh.ivvv.top

[R73] 分割大日志
来源：http://son.nanxinkj.top

split -l 1000 big.log part_
来源：http://ioj.yongpay.top

[R74] 批量重命名
来源：http://smf.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jdd.birdmap.top

[R75] 导出环境变量
来源：http://stv.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://ses.gotoacloud.top

[R76] 使用临时文件
来源：http://zxz.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iac.gotoacloud.top

[R77] 读取用户输入
来源：http://ich.aibaodan.cn

read -rp "请输入: " ans
来源：http://hda.zhixingplan.top

[R78] 交互式菜单
来源：http://wpo.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mcy.jyoumei.cn

[R79] 解析命令行选项
来源：http://rts.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://req.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://qml.zhongyouzk.top

time ./run.sh
来源：http://kef.sysykeji.top

================================================================================
来源：http://zdr.wangshuangyany.cn

S. C / C++ 专题
来源：http://fhs.hammf.cn

================================================================================
来源：http://nvt.zdbjq.cn

[S01] C：Hello World
来源：http://ghj.snrcjt.cn

#include <stdio.h>
来源：http://dgi.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xnc.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://kzo.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://hob.jqgfzy.top

[S03] C：读入整数
来源：http://sbc.yj202588.top

int x; scanf("%d", &x);
来源：http://hzo.hcnkem.com

[S04] C：字符串复制
来源：http://qwe.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://gpy.0kj1m.cn

[S05] C：字符串长度
来源：http://axo.tarul.cn

strlen(s)
来源：http://xha.hywenlv.cn

[S06] C：字符串比较
来源：http://vcw.9152youxi.cn

strcmp(a, b) == 0
来源：http://ztl.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://dhz.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yfg.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://tqq.mhx1999.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gsw.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://mnm.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mxr.cheryme.top

[S10] C：指针与解引用
来源：http://ynq.cashguo.top

int *p = &a;  *p = 5;
来源：http://iny.yj202588.top

[S11] C：逐行读文件
来源：http://ojm.shuidangran.top

FILE *f = fopen("a.txt", "r");
来源：http://rfe.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://enu.xziqi.cn

fclose(f);
来源：http://nep.jyoumei.cn

[S12] C：写文件
来源：http://dep.yueranfly.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zaj.chenlongwang.top

[S13] C：宏定义
来源：http://hzx.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yjy.shuidangran.top

[S14] C：枚举
来源：http://cff.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://ill.gzhubu.top

[S15] C：类型转换
来源：http://ene.yueranfly.top

(double) a / b
来源：http://cyd.9152youxi.cn

[S16] C：位操作置位
来源：http://wzh.tian-w.cn

x |= (1 << 3);
来源：http://yjs.nwbrower.top

[S17] C：安全拼接字符串
来源：http://alm.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jfy.yj20258888.top

[S18] C：命令行参数
来源：http://qyi.yongpay.top

int main(int argc, char **argv)
来源：http://xkh.bbcook.cn

[S19] C：快速排序
来源：http://epj.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://ers.xinyue.icu

[S20] C：二分查找
来源：http://lhv.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vpo.dashuyun.cn

[S21] C：字符类别判断
来源：http://nxy.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ypz.yuanzhike.top

[S22] C：字符串转数字
来源：http://lbe.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://csd.hnqzz.top

[S23] C：随机数
来源：http://ozo.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gto.birdmap.top

[S24] C：获取本地时间
来源：http://ujh.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bqr.meibo888.top

[S25] C：内存拷贝
来源：http://zvk.gzhubu.top

memcpy(dst, src, n);
来源：http://bju.jianghu66.top

[S26] C：内存清零
来源：http://lgr.hfpthk.cn

memset(a, 0, sizeof a);
来源：http://dsc.jinqigfzy.top

[S27] C：定义常量
来源：http://mhj.chenzaomai.com

const double PI = 3.14159;
来源：http://hzp.shzxlz.cn

[S28] C：静态变量
来源：http://lhy.cashguo.top

static int counter = 0;
来源：http://cqz.yueranfly.top

[S29] C：变参函数
来源：http://xcp.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jrm.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://evw.ivvv.top

#ifndef X_H
来源：http://fzi.birdmap.top

#define X_H
来源：http://frg.jqgfzy.top

#endif
来源：http://pfz.mhx1999.top

[S31] C++：Hello World
来源：http://btp.daxiang520.top

#include <iostream>
来源：http://fyx.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://qas.jyoumei.cn

[S32] C++：字符串
来源：http://zob.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://hyt.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://oav.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fft.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://vvi.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://bwu.yangfankeji.com

[S35] C++：map
来源：http://haj.sweek.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ahc.zhixingplan.top

[S36] C++：unordered_map
来源：http://usm.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vei.xuetiantiany.cn

[S37] C++：set
来源：http://rzd.sxryk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://elw.zhixingplan.top

[S38] C++：排序
来源：http://jhq.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://fwl.guowangkeji.top


<!-- 参考信息 -->