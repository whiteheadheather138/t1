代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bvw.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://mvl.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bur.yj20258.top

[Q57] 行号
来源：http://gyt.gaohongyu789.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xwa.yonumen.top

[Q58] 累计求和
来源：http://yeg.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aat.shzxlz.cn

[Q59] 分组内累计
来源：http://xxi.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lpe.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://opm.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qzv.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yec.sweek.top

[Q61] 移动平均
来源：http://rro.yj20258.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://msk.fanxiaobao.xyz

[Q62] 分组占比
来源：http://lkg.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rjn.yueranfly.top

[Q63] 开启事务
来源：http://tnr.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://alm.wangdashe.top

[Q64] 提交事务
来源：http://qpf.c1oappe.top

COMMIT;
来源：http://ior.zhijiandao.cn

[Q65] 回滚事务
来源：http://eev.cdnleiting.top

ROLLBACK;
来源：http://jne.cashguo.top

[Q66] 行锁查询
来源：http://dvd.sxryk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gzp.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://dqo.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bmz.xylfe.cn

[Q68] 保存点
来源：http://vgx.zhoulong.xyz

SAVEPOINT sp1;
来源：http://ffe.sufxvd.cn

ROLLBACK TO sp1;
来源：http://mio.xinyue.icu

[Q69] 查看执行计划
来源：http://bjf.yvedp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zhn.yangfankeji.com

[Q70] 更新统计信息
来源：http://gvv.hammf.cn

ANALYZE TABLE users;
来源：http://pyp.wangdashe.top

[Q71] 查看建表语句
来源：http://ltk.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://drw.bjfxy.top

[Q72] 查看索引
来源：http://bnf.redwolf501.top

SHOW INDEX FROM users;
来源：http://vqf.xuanzx.com

[Q73] 查看表状态
来源：http://qdo.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gac.hywenlv.cn

[Q74] 强制使用索引
来源：http://rom.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zjn.xuanzx.com

[Q75] 日期格式化
来源：http://uxx.jlsjyb.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ciu.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wwh.havefunace.top

[Q76] 按天统计
来源：http://llm.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tsk.yonumen.top

[Q77] 时间加减
来源：http://fyq.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uhp.jinqigfzy.top

[Q78] 当前时间
来源：http://nbw.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xla.yongpay.top

[Q79] 字符串拼接
来源：http://mzf.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vrj.yuxming.cn

[Q80] 字符串截取
来源：http://adf.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kue.jinqigfzy.top

[Q81] 字符串替换
来源：http://vii.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fwl.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://ggy.tianlin.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bih.yj202588.top

[Q83] 大小写转换
来源：http://pyi.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jyt.9152youxi.cn

[Q84] 去除首尾空格
来源：http://jcg.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://eud.chenzaomai.com

[Q85] 数值取整
来源：http://zws.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mrs.jyoumei.cn

[Q86] 读取 JSON 字段
来源：http://xyv.jlsjyb.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://squ.jyoumei.cn

[Q87] JSON 字段做条件
来源：http://gfd.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://twj.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://pmo.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eru.zhongyouzk.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uid.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://mad.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ofa.hnxiangtu.top

[Q90] 生成序号列
来源：http://nmx.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dsh.pycfn.com

================================================================================
来源：http://gza.smart0.xyz

R. Bash 专题
来源：http://rry.xylfe.cn

================================================================================
来源：http://qlo.feifeiyinyue.top

[R01] shebang 与严格模式
来源：http://knm.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://ohy.jinqigfzy.top

set -euo pipefail
来源：http://zko.cheryme.top

[R02] 变量赋值与使用
来源：http://bzu.daxiang520.top

name="Tom"; echo "$name"
来源：http://ikv.cqqwz.cn

[R03] 只读变量
来源：http://oco.ydjk.org.cn

readonly PI=3.14
来源：http://ovc.redwolf501.top

[R04] 位置参数
来源：http://xgn.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dwk.epnwcf.com

[R05] 参数默认值
来源：http://ohn.fktsv.cn

name="${1:-default}"
来源：http://bdu.cashguo.top

[R06] 判断命令是否存在
来源：http://ism.ctjpmb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://anm.dianchejie.cn

[R07] if 判断文件
来源：http://zuf.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sjg.yj202588.top

[R08] 数值比较
来源：http://rqh.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ddy.c1oappe.top

[R09] 字符串比较
来源：http://izp.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jfr.zhijiandao.cn

[R10] 正则匹配
来源：http://jwr.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baa.gotoacloud.top

[R11] case 多分支
来源：http://bym.yangfankeji.com

case "$1" in
来源：http://lux.sysykeji.top

start) echo "启动" ;;
来源：http://nif.xuanzx.com

stop)  echo "停止" ;;
来源：http://upv.jiagoushi.top

*)     echo "未知命令" ;;
来源：http://ahb.gotoacloud.top

esac
来源：http://lfo.hnqzz.top

[R12] for 遍历文件
来源：http://dyi.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://rst.hysaishi.cn

[R13] for 计数循环
来源：http://pce.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://ihe.gzhubu.top

[R14] C 风格 for
来源：http://qfn.epnwcf.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://isb.zhongyouzk.top

[R15] while 逐行读文件
来源：http://rub.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mlq.iojbl.cn

[R16] until 等待条件
来源：http://kcc.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rhy.zhengqikj.top

[R17] 数组定义与取值
来源：http://iez.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://zyd.xingfuxueyuan.xyz

[R18] 遍历数组
来源：http://zwv.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jst.gotoacloud.top

[R19] 数组长度
来源：http://pxs.daxiang520.top

echo "${#arr[@]}"
来源：http://esh.xuanzx.com

[R20] 关联数组（字典）
来源：http://nca.shzxlz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jou.dianchejie.cn

[R21] 字符串长度
来源：http://odj.ywan-chungtsiang.top

echo "${#s}"
来源：http://wbf.svipenyu.cn

[R22] 截取子串
来源：http://nwq.9152youxi.cn

echo "${s:0:5}"
来源：http://icc.chenjidiqi.icu

[R23] 字符串替换
来源：http://tpk.c1oappe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ibf.nwbrower.top

[R24] 大小写转换
来源：http://fjd.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kps.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://gde.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fdi.yuanzhike.top

[R26] 命令替换
来源：http://mjh.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://klx.yueranfly.top

[R27] 算术展开
来源：http://nbk.c1oappe.top

echo $((1 + 2 * 3))
来源：http://dyw.redwolf501.top

[R28] 浮点运算
来源：http://axb.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://fsg.chenzaomai.com

[R29] 定义函数
来源：http://pfr.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ezm.uphjek.com

[R30] 函数返回状态码
来源：http://mxo.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://smv.hammf.cn

[R31] 局部变量
来源：http://cuk.bbcook.cn

f() { local x=1; echo "$x"; }
来源：http://lfr.pengpengdd.cyou

[R32] 参数个数校验
来源：http://gyh.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rzv.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://ekk.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yvm.yuanzhike.top

[R34] 退出时清理
来源：http://vym.hesvh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lcv.sxryk.cn

[R35] 后台执行并等待
来源：http://czu.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gmv.zhengqikj.top

[R36] 并发执行多个任务
来源：http://fjm.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kpc.fehbvm.com

[R37] 把输出赋给变量
来源：http://lyt.aizwys.cn

files=$(ls -1)
来源：http://xgr.hywenlv.cn

[R38] 管道串联
来源：http://wmt.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://nsl.uphjek.com

[R39] 重定向标准输出与错误
来源：http://ahj.zdqjudy.top

cmd > out.log 2>&1
来源：http://mfd.yuanzhike.top

[R40] 追加写日志
来源：http://mou.jyoumei.cn

echo "log" >> out.log
来源：http://bgb.mhx1999.top

[R41] 丢弃输出
来源：http://sin.birdmap.top

cmd >/dev/null 2>&1
来源：http://txa.dianchejie.cn

[R42] 输入重定向
来源：http://zwc.meibo888.top

wc -l < a.txt
来源：http://gls.mhx1999.top

[R43] 按名字查找文件
来源：http://rwm.yueranfly.top

find . -name "*.log" -type f
来源：http://qzx.vehdjk.com

[R44] 按修改时间查找
来源：http://gut.zhijiandao.cn

find . -mtime -7 -type f
来源：http://mmi.jianghu66.top

[R45] 批量删除
来源：http://mqf.sufxvd.cn

find . -name "*.tmp" -delete
来源：http://tzm.yuxming.cn

[R46] 递归替换文件内容
来源：http://zrn.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tfp.ivvv.top

[R47] sed 单行替换
来源：http://miy.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://cut.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://hmn.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://ggi.gotoacloud.top

[R49] awk 带条件
来源：http://hvi.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zqf.zycfv.cn

[R50] awk 求和
来源：http://xiw.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hyg.smart0.xyz

[R51] 排序去重取前几
来源：http://itj.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://czm.daria6918.cn

[R52] 统计行数
来源：http://zby.ydjk.org.cn

wc -l a.txt
来源：http://dgc.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://lct.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zaz.xinyue.icu

[R54] 比较两个文件
来源：http://oef.zhengqikj.top

diff a.txt b.txt
来源：http://vyb.dianchejie.cn

[R55] 压缩与解压
来源：http://haf.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dmz.hfpthk.cn

[R56] 远程拷贝
来源：http://qae.hcnkem.com

scp file user@host:/path/
来源：http://eqp.zhoulong.xyz

[R57] 远程执行命令
来源：http://ivx.cashguo.top

ssh user@host 'uptime'
来源：http://ukh.jlsjyb.cn

[R58] 下载文件
来源：http://dpw.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kwe.tianlin.xyz

[R59] 发 POST JSON
来源：http://npv.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nfb.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://gzt.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nru.daria6918.cn

[R61] 磁盘占用
来源：http://nmm.hcnkem.com

df -h;  du -sh *
来源：http://lxy.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://kqw.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://tci.quarkkingdee.top

[R63] 内存与进程
来源：http://pzg.316326.xyz

free -h;  ps aux | grep nginx
来源：http://tor.fzhhl.top

[R64] 结束进程
来源：http://ejy.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://iiq.xinyue.icu

[R65] 查看端口占用
来源：http://gog.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ayv.chenlongwang.top

[R66] 定时任务
来源：http://lyu.gaohongyu789.top

crontab -e;  crontab -l
来源：http://bbd.ybcxt.top

[R67] 生成随机十六进制串
来源：http://vwi.havefunace.top

openssl rand -hex 16
来源：http://cis.smart0.xyz

[R68] 计算文件校验值
来源：http://jve.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://bro.ybcxt.top

[R69] 生成随机密码
来源：http://lpo.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://mjt.uphjek.com

[R70] 时间戳与互转
来源：http://lqo.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://xdw.yanxiufei.cn

[R71] 日期格式化
来源：http://nxu.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kig.havefunace.top

[R72] 等待端口就绪
来源：http://grg.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ggd.sysykeji.top

[R73] 分割大日志
来源：http://xxu.birdmap.top

split -l 1000 big.log part_
来源：http://mpn.vehdjk.com

[R74] 批量重命名
来源：http://tji.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hyd.havefunace.top

[R75] 导出环境变量
来源：http://sat.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://zgu.jyoumei.cn

[R76] 使用临时文件
来源：http://qyu.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aiq.nanxuanxn.top

[R77] 读取用户输入
来源：http://dvd.kuanghao11.cn

read -rp "请输入: " ans
来源：http://xsu.yuxming.cn

[R78] 交互式菜单
来源：http://wiy.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://byh.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://ypj.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rhv.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://lib.yanxiufei.cn

time ./run.sh
来源：http://sms.nanxuanxn.top

================================================================================
来源：http://end.jqgufenzy.top

S. C / C++ 专题
来源：http://gjy.zhoulong.xyz

================================================================================
来源：http://rxc.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://rnj.ybcxt.top

#include <stdio.h>
来源：http://fjy.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lfx.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://jrj.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://ioh.ctjpmb.com

[S03] C：读入整数
来源：http://wzw.jinqigufen.top

int x; scanf("%d", &x);
来源：http://oze.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://deo.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://dbx.jinqigfzy.top

[S05] C：字符串长度
来源：http://ieo.ybcxt.top

strlen(s)
来源：http://vld.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://dde.316326.xyz

strcmp(a, b) == 0
来源：http://dip.cheryme.top

[S07] C：数组遍历求和
来源：http://pbv.wangdashe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mrg.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://wgt.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jfo.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://gqt.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zyd.daria6918.cn

[S10] C：指针与解引用
来源：http://fsz.tarul.cn

int *p = &a;  *p = 5;
来源：http://xsp.yangfankeji.com

[S11] C：逐行读文件
来源：http://zff.yj20258888.top

FILE *f = fopen("a.txt", "r");
来源：http://yha.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lvn.haohaochexian.top

fclose(f);
来源：http://lko.zdbjq.cn

[S12] C：写文件
来源：http://bvr.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xcf.zdqjudy.top

[S13] C：宏定义
来源：http://qoi.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lbb.chenzaomai.com

[S14] C：枚举
来源：http://yti.hammf.cn

enum Color { RED, GREEN, BLUE };
来源：http://tft.zhengqikj.top

[S15] C：类型转换
来源：http://unb.yfazqb.com

(double) a / b
来源：http://zoa.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://lyy.shzxlz.cn

x |= (1 << 3);
来源：http://akj.xuanzx.com

[S17] C：安全拼接字符串
来源：http://eev.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sql.daxiang520.top

[S18] C：命令行参数
来源：http://dqn.tanke756.top

int main(int argc, char **argv)
来源：http://pcw.jlsjyb.cn

[S19] C：快速排序
来源：http://dqy.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://qrb.yangfankeji.com

[S20] C：二分查找
来源：http://yvz.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cca.jlsjyb.cn

[S21] C：字符类别判断
来源：http://mnl.sweek.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nbc.sxryk.cn

[S22] C：字符串转数字
来源：http://xfp.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ahv.shzxlz.cn

[S23] C：随机数
来源：http://jxb.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cdt.vqdsnc.cn

[S24] C：获取本地时间
来源：http://zej.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ehg.nwbrower.top

[S25] C：内存拷贝
来源：http://esg.epnwcf.com

memcpy(dst, src, n);
来源：http://gao.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://dpn.zycfv.cn


<!-- 参考信息 -->