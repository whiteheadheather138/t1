代发 wailian999

[Q63] 开启事务
来源：http://omf.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://wfy.hywenlv.cn

[Q64] 提交事务
来源：http://voq.pengpengdd.cyou

COMMIT;
来源：http://hxx.xuetiantiany.cn

[Q65] 回滚事务
来源：http://bsp.hcnkem.com

ROLLBACK;
来源：http://igg.hcnkem.com

[Q66] 行锁查询
来源：http://dmm.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yuh.ydzc1.top

[Q67] 设置隔离级别
来源：http://slc.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zkj.nanxinkj.top

[Q68] 保存点
来源：http://utm.shuidangran.top

SAVEPOINT sp1;
来源：http://oag.guannengcc.top

ROLLBACK TO sp1;
来源：http://enx.ywan-chungtsiang.top

[Q69] 查看执行计划
来源：http://qdw.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oju.zhongyouzk.top

[Q70] 更新统计信息
来源：http://gwb.ybcxt.top

ANALYZE TABLE users;
来源：http://otq.jianghu66.top

[Q71] 查看建表语句
来源：http://pnn.jiagoushi.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nxl.hywenlv.cn

[Q72] 查看索引
来源：http://srg.redwolf501.top

SHOW INDEX FROM users;
来源：http://zfa.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://voe.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yvq.andypj.xyz

[Q74] 强制使用索引
来源：http://pbw.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zen.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://fah.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wgl.bjfxy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jqs.cucudq.cn

[Q76] 按天统计
来源：http://abf.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cvb.0kj1m.cn

[Q77] 时间加减
来源：http://ugo.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qjd.ctjpmb.com

[Q78] 当前时间
来源：http://fee.hnxiangtu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qin.epnwcf.com

[Q79] 字符串拼接
来源：http://lhg.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mad.fehbvm.com

[Q80] 字符串截取
来源：http://ctt.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mhk.bjfxy.top

[Q81] 字符串替换
来源：http://pzg.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://duu.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://jzs.kuanghao11.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bmn.sufxvd.cn

[Q83] 大小写转换
来源：http://zga.gzhubu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uon.jqgfzy.top

[Q84] 去除首尾空格
来源：http://elo.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://dva.yonumen.top

[Q85] 数值取整
来源：http://oog.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://brc.hammf.cn

[Q86] 读取 JSON 字段
来源：http://yyb.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tgi.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://ast.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://crp.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://qtm.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pmq.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gva.fengsongda.top

[Q89] 判断表是否存在
来源：http://lga.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qst.sweek.top

[Q90] 生成序号列
来源：http://wol.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fal.nanxinkj.top

================================================================================
来源：http://eey.ppjwa.cn

R. Bash 专题
来源：http://isf.zdbjq.cn

================================================================================
来源：http://cbe.redwolf501.top

[R01] shebang 与严格模式
来源：http://dpj.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://ilw.gogol.net.cn

set -euo pipefail
来源：http://phh.hnqzz.top

[R02] 变量赋值与使用
来源：http://afv.jiagoushi.top

name="Tom"; echo "$name"
来源：http://hwn.hongshengwenyu.top

[R03] 只读变量
来源：http://dog.vqdsnc.cn

readonly PI=3.14
来源：http://vnq.xziqi.cn

[R04] 位置参数
来源：http://snl.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cnm.iojbl.cn

[R05] 参数默认值
来源：http://bai.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://jzf.316326.xyz

[R06] 判断命令是否存在
来源：http://cph.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vyh.aizwys.cn

[R07] if 判断文件
来源：http://zpk.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lli.sxryk.cn

[R08] 数值比较
来源：http://igk.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wpw.jqgufenzy.top

[R09] 字符串比较
来源：http://ngh.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://csk.jianghu66.top

[R10] 正则匹配
来源：http://hpy.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kwt.cucudq.cn

[R11] case 多分支
来源：http://dvf.pengpengdd.cyou

case "$1" in
来源：http://sfz.iojbl.cn

start) echo "启动" ;;
来源：http://ihs.gogol.net.cn

stop)  echo "停止" ;;
来源：http://uhm.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://moj.tanke756.top

esac
来源：http://lgx.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://hcy.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://eou.dashuyun.cn

[R13] for 计数循环
来源：http://sqj.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://xfw.tian-w.cn

[R14] C 风格 for
来源：http://zbt.yvedp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fnt.zycfv.cn

[R15] while 逐行读文件
来源：http://bbq.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zss.nwbrower.top

[R16] until 等待条件
来源：http://cxe.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qsd.fktsv.cn

[R17] 数组定义与取值
来源：http://zwj.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wtf.9152youxi.cn

[R18] 遍历数组
来源：http://myk.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cnq.jinqigfzy.top

[R19] 数组长度
来源：http://vpm.redwolf501.top

echo "${#arr[@]}"
来源：http://ici.nanxinkj.top

[R20] 关联数组（字典）
来源：http://xlb.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wgf.chenlongwang.top

[R21] 字符串长度
来源：http://dhi.jqgfzy.top

echo "${#s}"
来源：http://gzs.mhx1999.top

[R22] 截取子串
来源：http://msd.kuanghao11.cn

echo "${s:0:5}"
来源：http://pbf.yangfankeji.com

[R23] 字符串替换
来源：http://man.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kew.zhiwuduotai.top

[R24] 大小写转换
来源：http://lyv.jinqigfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://lqn.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://azw.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uox.nanxuanxn.top

[R26] 命令替换
来源：http://qqk.cdnleiting.top

now=$(date +%F); echo "$now"
来源：http://eye.gogol.net.cn

[R27] 算术展开
来源：http://hzk.quarkkingdee.top

echo $((1 + 2 * 3))
来源：http://mmt.jqgufenzy.top

[R28] 浮点运算
来源：http://xlo.tarul.cn

echo "scale=2; 10/3" | bc
来源：http://hsh.jianghu66.top

[R29] 定义函数
来源：http://nla.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cax.hnxiangtu.top

[R30] 函数返回状态码
来源：http://tzr.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://anv.feifeiyinyue.top

[R31] 局部变量
来源：http://kuh.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://imi.ydjk.org.cn

[R32] 参数个数校验
来源：http://dvy.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jlv.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://jet.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://evf.ivvv.top

[R34] 退出时清理
来源：http://kyf.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://kbv.ybcxt.top

[R35] 后台执行并等待
来源：http://ucz.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://vsd.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://kti.meibo888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mbg.sysykeji.top

[R37] 把输出赋给变量
来源：http://yrt.guowangkeji.top

files=$(ls -1)
来源：http://iuq.meibo888.top

[R38] 管道串联
来源：http://qnk.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://dok.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://yde.yanxiufei.cn

cmd > out.log 2>&1
来源：http://knu.pengpengdd.cyou

[R40] 追加写日志
来源：http://wyb.hywenlv.cn

echo "log" >> out.log
来源：http://kdw.jinqigfzy.top

[R41] 丢弃输出
来源：http://gbc.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://nyz.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://par.yonumen.top

wc -l < a.txt
来源：http://mju.jqgufenzy.top

[R43] 按名字查找文件
来源：http://vom.fzhhl.top

find . -name "*.log" -type f
来源：http://uvv.birdmap.top

[R44] 按修改时间查找
来源：http://csv.yj20258888.top

find . -mtime -7 -type f
来源：http://cux.yonumen.top

[R45] 批量删除
来源：http://xhy.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://dpj.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://oko.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hoa.ctjpmb.com

[R47] sed 单行替换
来源：http://iwk.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://lew.xziqi.cn

[R48] awk 取指定列
来源：http://nkn.snrcjt.cn

awk '{print $1, $3}' a.txt
来源：http://fek.zdqjudy.top

[R49] awk 带条件
来源：http://cqw.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://acw.tian-w.cn

[R50] awk 求和
来源：http://tma.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://prh.mhx1999.top

[R51] 排序去重取前几
来源：http://oms.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uta.gogol.net.cn

[R52] 统计行数
来源：http://ddz.yueranfly.top

wc -l a.txt
来源：http://pcz.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://oqx.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nni.ybcxt.top

[R54] 比较两个文件
来源：http://erp.yueranfly.top

diff a.txt b.txt
来源：http://txy.hysaishi.cn

[R55] 压缩与解压
来源：http://wnj.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yrv.zhixingplan.top

[R56] 远程拷贝
来源：http://bna.bjfxy.top

scp file user@host:/path/
来源：http://hgu.jqgufenzy.top

[R57] 远程执行命令
来源：http://vwr.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://srm.aizwys.cn

[R58] 下载文件
来源：http://bkg.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ydp.havefunace.top

[R59] 发 POST JSON
来源：http://fbl.bjfxy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://adt.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://sud.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ggr.zdqjudy.top

[R61] 磁盘占用
来源：http://cyf.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://yfm.yangfankeji.com

[R62] 找最占空间的文件
来源：http://sya.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://dgi.yj20258.top

[R63] 内存与进程
来源：http://uef.havefunace.top

free -h;  ps aux | grep nginx
来源：http://mpv.hesvh.cn

[R64] 结束进程
来源：http://tbh.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://uld.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://yvm.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wzq.ppjwa.cn

[R66] 定时任务
来源：http://fyo.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://dib.cashguo.top

[R67] 生成随机十六进制串
来源：http://qdb.zhoulong.xyz

openssl rand -hex 16
来源：http://rrt.cheryme.top

[R68] 计算文件校验值
来源：http://ord.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://pzx.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://ymr.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://xhx.wangdashe.top

[R70] 时间戳与互转
来源：http://jng.xinyue.icu

date +%s;  date -d @1700000000
来源：http://jlh.smart0.xyz

[R71] 日期格式化
来源：http://zgh.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lci.epnwcf.com

[R72] 等待端口就绪
来源：http://col.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lra.uphjek.com

[R73] 分割大日志
来源：http://qvz.tarul.cn

split -l 1000 big.log part_
来源：http://ltl.yuxming.cn

[R74] 批量重命名
来源：http://jcy.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://icw.fengsongda.top

[R75] 导出环境变量
来源：http://zta.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://xso.cheryme.top

[R76] 使用临时文件
来源：http://zkr.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zos.0kj1m.cn

[R77] 读取用户输入
来源：http://tqk.hywenlv.cn

read -rp "请输入: " ans
来源：http://atr.sjlbkw.cn

[R78] 交互式菜单
来源：http://zqz.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://qtv.havefunace.top

[R79] 解析命令行选项
来源：http://nsq.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://crc.yongpay.top

[R80] 查看脚本执行耗时
来源：http://afo.aibaodan.cn

time ./run.sh
来源：http://mmh.xylfe.cn

================================================================================
来源：http://yfw.jqgfzy.top

S. C / C++ 专题
来源：http://mrk.yonumen.top

================================================================================
来源：http://bwm.shangyingyoupin.top

[S01] C：Hello World
来源：http://dye.jinqigufen.top

#include <stdio.h>
来源：http://frh.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qdw.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://hxh.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://cwh.chenjidiqi.icu

[S03] C：读入整数
来源：http://hsp.cqqwz.cn

int x; scanf("%d", &x);
来源：http://udq.hfpthk.cn

[S04] C：字符串复制
来源：http://riu.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gtf.vqdsnc.cn

[S05] C：字符串长度
来源：http://bsa.epnwcf.com

strlen(s)
来源：http://opf.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://xce.yvedp.cn

strcmp(a, b) == 0
来源：http://ihs.xylfe.cn

[S07] C：数组遍历求和
来源：http://tdi.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sod.tanke756.top

[S08] C：动态内存分配与释放
来源：http://vre.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://has.uphjek.com

[S09] C：结构体定义与初始化
来源：http://izb.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yds.ydjk.org.cn

[S10] C：指针与解引用
来源：http://goc.xylfe.cn

int *p = &a;  *p = 5;
来源：http://lne.wangdashe.top

[S11] C：逐行读文件
来源：http://llt.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://dyl.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dqk.nwbrower.top

fclose(f);
来源：http://zcz.xylfe.cn

[S12] C：写文件
来源：http://unj.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rgt.yonumen.top

[S13] C：宏定义
来源：http://mno.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zpk.pycfn.com

[S14] C：枚举
来源：http://ucr.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://ozv.cdnleiting.top

[S15] C：类型转换
来源：http://tad.guannengcc.top

(double) a / b
来源：http://fuy.fehbvm.com

[S16] C：位操作置位
来源：http://nao.sweek.top

x |= (1 << 3);
来源：http://wbr.ydzc1.top

[S17] C：安全拼接字符串
来源：http://imh.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://okd.chenlongwang.top

[S18] C：命令行参数
来源：http://gvf.cheryme.top

int main(int argc, char **argv)
来源：http://sdn.sweek.top

[S19] C：快速排序
来源：http://bua.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://mgt.andypj.xyz

[S20] C：二分查找
来源：http://yye.feifeiyinyue.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zln.sysykeji.top

[S21] C：字符类别判断
来源：http://udr.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://irt.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://nmy.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://lsi.dianchejie.cn

[S23] C：随机数
来源：http://xtu.0kj1m.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://scq.epnwcf.com

[S24] C：获取本地时间
来源：http://dkl.andypj.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fuu.ybcxt.top

[S25] C：内存拷贝
来源：http://mqt.xuanzx.com

memcpy(dst, src, n);
来源：http://yrf.tianlin.xyz

[S26] C：内存清零
来源：http://azp.9152youxi.cn

memset(a, 0, sizeof a);
来源：http://qjg.feifeiyinyue.top

[S27] C：定义常量
来源：http://urx.guannengcc.top

const double PI = 3.14159;
来源：http://imn.zhaomingkeji.xyz

[S28] C：静态变量
来源：http://mtt.andypj.xyz

static int counter = 0;
来源：http://zxi.zhiwuduotai.top

[S29] C：变参函数
来源：http://tea.yangfankeji.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kfv.vqdsnc.cn

[S30] C：头文件保护
来源：http://ixt.jiagoushi.top

#ifndef X_H
来源：http://qhw.kuanghao11.cn

#define X_H
来源：http://znu.shanyushiyangtech.top

#endif
来源：http://mjr.hnxiangtu.top

[S31] C++：Hello World
来源：http://zjl.bjfxy.top

#include <iostream>
来源：http://mgi.zhoulong.xyz

int main() { std::cout << "Hello\n"; }
来源：http://nvb.jyoumei.cn

[S32] C++：字符串
来源：http://ngq.316326.xyz

std::string s = "hi";  s += "!";
来源：http://kkq.smart0.xyz


<!-- 参考信息 -->