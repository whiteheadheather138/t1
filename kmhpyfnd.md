代发 wailian999

[Q61] 移动平均
来源：http://bki.yonumen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ooi.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://qbm.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ewf.gogol.net.cn

[Q63] 开启事务
来源：http://mpm.ydzc1.top

START TRANSACTION;                -- 或 BEGIN
来源：http://joo.nanxinkj.top

[Q64] 提交事务
来源：http://jfc.tian-w.cn

COMMIT;
来源：http://htr.daxiang520.top

[Q65] 回滚事务
来源：http://mho.shuidangran.top

ROLLBACK;
来源：http://lei.xziqi.cn

[Q66] 行锁查询
来源：http://lph.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ugg.yvedp.cn

[Q67] 设置隔离级别
来源：http://yld.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iqd.ybcxt.top

[Q68] 保存点
来源：http://oau.xuetiantiany.cn

SAVEPOINT sp1;
来源：http://exw.gzhubu.top

ROLLBACK TO sp1;
来源：http://bdy.aibaodan.cn

[Q69] 查看执行计划
来源：http://nvu.zhiwuduotai.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ymw.jinqigfzy.top

[Q70] 更新统计信息
来源：http://pxb.bjfxy.top

ANALYZE TABLE users;
来源：http://inv.uphjek.com

[Q71] 查看建表语句
来源：http://zfy.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kdf.cheryme.top

[Q72] 查看索引
来源：http://xbh.jinqigufen.top

SHOW INDEX FROM users;
来源：http://kuc.sweek.top

[Q73] 查看表状态
来源：http://ulg.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jee.sufxvd.cn

[Q74] 强制使用索引
来源：http://ant.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xno.hammf.cn

[Q75] 日期格式化
来源：http://ues.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xii.jinqigufen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oxd.jinghuilouyu.cn

[Q76] 按天统计
来源：http://bag.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://opp.hnxiangtu.top

[Q77] 时间加减
来源：http://eyh.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bzz.ivvv.top

[Q78] 当前时间
来源：http://eqk.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uua.xziqi.cn

[Q79] 字符串拼接
来源：http://zis.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rst.zhiwuduotai.top

[Q80] 字符串截取
来源：http://krf.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bdw.pycfn.com

[Q81] 字符串替换
来源：http://ynx.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mxb.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://dso.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rye.dashuyun.cn

[Q83] 大小写转换
来源：http://vtm.jinghuilouyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eah.yfazqb.com

[Q84] 去除首尾空格
来源：http://spz.shzxlz.cn

SELECT TRIM(name) FROM users;
来源：http://hki.tarul.cn

[Q85] 数值取整
来源：http://ern.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qjv.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://gdc.shzxlz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xsd.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://zxy.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wno.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://vdp.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xwo.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://njd.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://etd.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mby.iojbl.cn

[Q90] 生成序号列
来源：http://stn.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mlu.ydjk.org.cn

================================================================================
来源：http://bwu.nanxuanxn.top

R. Bash 专题
来源：http://dsb.svipenyu.cn

================================================================================
来源：http://frs.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://qys.gotoacloud.top

#!/usr/bin/env bash
来源：http://gos.ybcxt.top

set -euo pipefail
来源：http://idv.52xcode.cn

[R02] 变量赋值与使用
来源：http://ird.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://grm.hesvh.cn

[R03] 只读变量
来源：http://xbq.hfpthk.cn

readonly PI=3.14
来源：http://lhb.wangshuangyany.cn

[R04] 位置参数
来源：http://max.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aoa.tarul.cn

[R05] 参数默认值
来源：http://jmy.iojbl.cn

name="${1:-default}"
来源：http://pvw.shzxlz.cn

[R06] 判断命令是否存在
来源：http://ggm.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sxl.sweek.top

[R07] if 判断文件
来源：http://wym.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xhx.yonumen.top

[R08] 数值比较
来源：http://brk.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pvr.ybcxt.top

[R09] 字符串比较
来源：http://oih.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pmu.andypj.xyz

[R10] 正则匹配
来源：http://xat.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://twp.ybcxt.top

[R11] case 多分支
来源：http://odu.kuanghao11.cn

case "$1" in
来源：http://xin.yanxiufei.cn

start) echo "启动" ;;
来源：http://tbq.fehbvm.com

stop)  echo "停止" ;;
来源：http://joy.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://lbu.xingfuxueyuan.xyz

esac
来源：http://ejw.yvedp.cn

[R12] for 遍历文件
来源：http://tyi.ybcxt.top

for f in *.txt; do echo "$f"; done
来源：http://wdc.yj20258.top

[R13] for 计数循环
来源：http://uud.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://mzw.pycfn.com

[R14] C 风格 for
来源：http://nlx.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kxk.cqqwz.cn

[R15] while 逐行读文件
来源：http://vtk.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qev.yangfankeji.com

[R16] until 等待条件
来源：http://jvm.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hez.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://ssn.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://nzy.yongpay.top

[R18] 遍历数组
来源：http://ncd.hywenlv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lgf.hnxiangtu.top

[R19] 数组长度
来源：http://gub.svipenyu.cn

echo "${#arr[@]}"
来源：http://yph.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://rmx.shzxlz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://esg.nanxinkj.top

[R21] 字符串长度
来源：http://ogj.yueranfly.top

echo "${#s}"
来源：http://rmp.shzxlz.cn

[R22] 截取子串
来源：http://idc.cucudq.cn

echo "${s:0:5}"
来源：http://bwb.aizwys.cn

[R23] 字符串替换
来源：http://wgg.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ewt.wangshuangyany.cn

[R24] 大小写转换
来源：http://inq.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://yju.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://nrg.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xix.vqdsnc.cn

[R26] 命令替换
来源：http://nww.jyoumei.cn

now=$(date +%F); echo "$now"
来源：http://utk.ywan-chungtsiang.top

[R27] 算术展开
来源：http://vra.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://baf.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://sjz.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://vgg.tianlin.xyz

[R29] 定义函数
来源：http://hoe.fengsongda.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fwt.jinqigfzy.top

[R30] 函数返回状态码
来源：http://oid.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://koo.jianghu66.top

[R31] 局部变量
来源：http://dxu.jinyuanbaomall.cn

f() { local x=1; echo "$x"; }
来源：http://vll.vehdjk.com

[R32] 参数个数校验
来源：http://bku.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ebb.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://mbk.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://utq.aibaodan.cn

[R34] 退出时清理
来源：http://blo.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://jpr.xinyue.icu

[R35] 后台执行并等待
来源：http://eor.ybcxt.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nns.wangdashe.top

[R36] 并发执行多个任务
来源：http://xdx.xinyue.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kvp.nwbrower.top

[R37] 把输出赋给变量
来源：http://ltq.daxiang520.top

files=$(ls -1)
来源：http://ruv.zhengqikj.top

[R38] 管道串联
来源：http://hhg.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://jjb.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://rex.gotoacloud.top

cmd > out.log 2>&1
来源：http://uri.sysykeji.top

[R40] 追加写日志
来源：http://kna.yj202588.top

echo "log" >> out.log
来源：http://knl.jianghu66.top

[R41] 丢弃输出
来源：http://mqb.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://zgy.gotoacloud.top

[R42] 输入重定向
来源：http://lso.zhaomingkeji.xyz

wc -l < a.txt
来源：http://veo.cdnleiting.top

[R43] 按名字查找文件
来源：http://ckn.316326.xyz

find . -name "*.log" -type f
来源：http://ppf.ppjwa.cn

[R44] 按修改时间查找
来源：http://hlr.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://qqy.fengsongda.top

[R45] 批量删除
来源：http://pqk.mhx1999.top

find . -name "*.tmp" -delete
来源：http://ecc.ybcxt.top

[R46] 递归替换文件内容
来源：http://yss.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vfg.chenzaomai.com

[R47] sed 单行替换
来源：http://eof.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yor.tianlin.xyz

[R48] awk 取指定列
来源：http://mrs.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://kua.guannengcc.top

[R49] awk 带条件
来源：http://lth.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sti.fanxiaobao.xyz

[R50] awk 求和
来源：http://bkn.tian-w.cn

awk '{s += $2} END {print s}' a.txt
来源：http://drf.c1oappe.top

[R51] 排序去重取前几
来源：http://szl.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://joq.sufxvd.cn

[R52] 统计行数
来源：http://jyt.smart0.xyz

wc -l a.txt
来源：http://pda.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://vnr.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mcs.smart0.xyz

[R54] 比较两个文件
来源：http://snd.hammf.cn

diff a.txt b.txt
来源：http://mqj.yuanzhike.top

[R55] 压缩与解压
来源：http://fan.yj20258888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qdb.jinqigufen.top

[R56] 远程拷贝
来源：http://zqt.sysykeji.top

scp file user@host:/path/
来源：http://dyk.gogol.net.cn

[R57] 远程执行命令
来源：http://bvm.ydzc1.top

ssh user@host 'uptime'
来源：http://wqm.xuetiantiany.cn

[R58] 下载文件
来源：http://vns.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zrm.haohaochexian.top

[R59] 发 POST JSON
来源：http://sbn.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jjs.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://gys.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wcn.kuanghao11.cn

[R61] 磁盘占用
来源：http://cbn.andypj.xyz

df -h;  du -sh *
来源：http://ddj.smart0.xyz

[R62] 找最占空间的文件
来源：http://plb.daria6918.cn

du -ah . | sort -rh | head -10
来源：http://dbq.yueranfly.top

[R63] 内存与进程
来源：http://bdc.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://ygp.meibo888.top

[R64] 结束进程
来源：http://uan.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://wsd.cdnleiting.top

[R65] 查看端口占用
来源：http://ljl.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tuv.fanxiaobao.xyz

[R66] 定时任务
来源：http://uzm.jinqigfzy.top

crontab -e;  crontab -l
来源：http://eum.yvedp.cn

[R67] 生成随机十六进制串
来源：http://vfx.zhiwuduotai.top

openssl rand -hex 16
来源：http://kri.52xcode.cn

[R68] 计算文件校验值
来源：http://iue.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://cio.iojbl.cn

[R69] 生成随机密码
来源：http://zjo.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://zah.yfazqb.com

[R70] 时间戳与互转
来源：http://mew.cheryme.top

date +%s;  date -d @1700000000
来源：http://epe.kuanghao11.cn

[R71] 日期格式化
来源：http://jjf.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rlq.hywenlv.cn

[R72] 等待端口就绪
来源：http://eip.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://atl.zhijiandao.cn

[R73] 分割大日志
来源：http://mpz.jlsjyb.cn

split -l 1000 big.log part_
来源：http://sej.jianghu66.top

[R74] 批量重命名
来源：http://fsd.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ozm.ybcxt.top

[R75] 导出环境变量
来源：http://fqz.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://fss.zhiwuduotai.top

[R76] 使用临时文件
来源：http://xqr.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hpf.zhengqikj.top

[R77] 读取用户输入
来源：http://dsm.vqdsnc.cn

read -rp "请输入: " ans
来源：http://fbx.redwolf501.top

[R78] 交互式菜单
来源：http://shh.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ntn.sweek.top

[R79] 解析命令行选项
来源：http://sgk.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://noa.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://wjz.jiagoushi.top

time ./run.sh
来源：http://lsq.jiagoushi.top

================================================================================
来源：http://pxp.tarul.cn

S. C / C++ 专题
来源：http://tnf.nanxuanxn.top

================================================================================
来源：http://bsn.birdmap.top

[S01] C：Hello World
来源：http://hai.iojbl.cn

#include <stdio.h>
来源：http://dce.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.cucudq.cn

[S02] C：变量与格式化输出
来源：http://frl.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://hht.jlsjyb.cn

[S03] C：读入整数
来源：http://ohs.quarkkingdee.top

int x; scanf("%d", &x);
来源：http://inu.xuetiantiany.cn

[S04] C：字符串复制
来源：http://ytk.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://dxt.bbcook.cn

[S05] C：字符串长度
来源：http://rej.zhongyouzk.top

strlen(s)
来源：http://xyu.zdqjudy.top

[S06] C：字符串比较
来源：http://lrl.haohaochexian.top

strcmp(a, b) == 0
来源：http://cma.yangfankeji.com

[S07] C：数组遍历求和
来源：http://jnr.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xhq.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://azl.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ruf.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://uqx.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hoi.yj20258888.top

[S10] C：指针与解引用
来源：http://awy.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://iix.uphjek.com

[S11] C：逐行读文件
来源：http://exn.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://dyn.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://arw.cqqwz.cn

fclose(f);
来源：http://ztr.gogol.net.cn

[S12] C：写文件
来源：http://inq.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aez.ydjk.org.cn

[S13] C：宏定义
来源：http://zrb.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kjy.jinyuanbaomall.cn

[S14] C：枚举
来源：http://apx.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://aji.cucudq.cn

[S15] C：类型转换
来源：http://esh.gzhubu.top

(double) a / b
来源：http://bzx.snrcjt.cn

[S16] C：位操作置位
来源：http://zfn.ctjpmb.com

x |= (1 << 3);
来源：http://akp.daria6918.cn

[S17] C：安全拼接字符串
来源：http://nnl.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qve.guannengcc.top

[S18] C：命令行参数
来源：http://hil.guowangkeji.top

int main(int argc, char **argv)
来源：http://vob.zhongyouzk.top

[S19] C：快速排序
来源：http://jtt.nanxuanxn.top

qsort(a, n, sizeof(int), cmp);
来源：http://xlx.zdqjudy.top

[S20] C：二分查找
来源：http://ywv.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ivk.gzhubu.top

[S21] C：字符类别判断
来源：http://ucp.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xjq.hnxiangtu.top

[S22] C：字符串转数字
来源：http://ndv.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://adt.ydjk.org.cn

[S23] C：随机数
来源：http://ypi.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mpm.yueranfly.top

[S24] C：获取本地时间
来源：http://pmk.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gcj.haohaochexian.top

[S25] C：内存拷贝
来源：http://ltf.shzxlz.cn

memcpy(dst, src, n);
来源：http://qjk.gzhubu.top

[S26] C：内存清零
来源：http://nhx.bbcook.cn

memset(a, 0, sizeof a);
来源：http://fcu.zhixingplan.top

[S27] C：定义常量
来源：http://csj.zhijiandao.cn

const double PI = 3.14159;
来源：http://ikk.316326.xyz

[S28] C：静态变量
来源：http://hee.jyoumei.cn

static int counter = 0;
来源：http://jmj.gotoacloud.top

[S29] C：变参函数
来源：http://osp.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dry.chenzaomai.com

[S30] C：头文件保护
来源：http://hzt.shzxlz.cn

#ifndef X_H
来源：http://xtp.tian-w.cn

#define X_H
来源：http://ktf.yvedp.cn

#endif
来源：http://roy.zhoulong.xyz

[S31] C++：Hello World
来源：http://ffh.xinyue.icu


<!-- 参考信息 -->